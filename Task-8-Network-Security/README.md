# Network Security Concepts and Firewall Basics

# Introduction

Network security protects computer networks from unauthorized access, attacks, and data theft. Firewalls, IDS/IPS systems, VPNs, and packet analysis tools are essential for securing modern networks.

---

# 1. Types of Firewalls

## Packet Filtering Firewall

A packet filtering firewall examines packets based on source IP, destination IP, port number, and protocol. It allows or blocks traffic according to predefined rules.

### Advantages

* Fast
* Simple configuration

### Disadvantages

* Cannot inspect application data

---

## Stateful Firewall

A stateful firewall tracks active network connections and only allows packets that belong to valid sessions.

### Advantages

* More secure than packet filtering
* Tracks connection state

### Disadvantages

* Uses more system resources

---

## Application Layer Firewall

An application layer firewall inspects traffic at the application level (Layer 7), such as HTTP and FTP.

### Advantages

* Detects application attacks
* Filters malicious requests

### Disadvantages

* Slower than other firewall types

---

# 2. Basic iptables Rules

## Allow SSH (Port 22)

```bash
sudo iptables -A INPUT -p tcp --dport 22 -j ACCEPT
```

---

## Allow HTTP (Port 80)

```bash
sudo iptables -A INPUT -p tcp --dport 80 -j ACCEPT
```

---

## Allow HTTPS (Port 443)

```bash
sudo iptables -A INPUT -p tcp --dport 443 -j ACCEPT
```

---

## Block Telnet (Port 23)

```bash
sudo iptables -A INPUT -p tcp --dport 23 -j DROP
```

---

## View Rules

```bash
sudo iptables -L
```

<img width="518" height="411" alt="image" src="https://github.com/user-attachments/assets/080dc78a-0f7d-4aa0-9e84-1fbe59b60435" />

---

# 3. IDS and IPS

## Intrusion Detection System (IDS)

An IDS monitors network traffic and generates alerts when suspicious activity is detected.

### Example

Snort

<img width="1907" height="942" alt="image" src="https://github.com/user-attachments/assets/d309a862-0810-4477-bbb5-7463db35f5c8" />

---

## Intrusion Prevention System (IPS)

An IPS detects and automatically blocks malicious traffic.

### Example

Suricata

<img width="1909" height="886" alt="image" src="https://github.com/user-attachments/assets/1e0fec17-308a-426d-a80b-bedcc99a105d" />

---

# Difference Between IDS and IPS

| IDS             | IPS                        |
| --------------- | -------------------------- |
| Detects attacks | Detects and blocks attacks |
| Sends alerts    | Takes preventive action    |
| Passive         | Active                     |

---

# 4. VPN

A Virtual Private Network (VPN) encrypts internet traffic between a device and a VPN server.

## Benefits

* Protects privacy
* Encrypts network traffic
* Hides public IP address
* Secures remote access

<img width="1919" height="454" alt="image" src="https://github.com/user-attachments/assets/0abcecac-e65e-4fc7-96d3-5c42f84e6514" />

---

# 5. Wireshark Packet Analysis

Wireshark is a network protocol analyzer used to inspect network traffic.

## Basic Steps

1. Open a packet capture (.pcap) file.
2. Apply filters.
3. Analyze packets.
4. Identify suspicious traffic.

<img width="1914" height="942" alt="image" src="https://github.com/user-attachments/assets/42a67f57-3049-4cdd-8230-7a78df2c433e" />

---

# 6. Suspicious Traffic Patterns

Examples include:

* Large number of failed login attempts
* Unexpected traffic to unknown IP addresses
* Port scanning activity
* Repeated DNS requests
* High outbound traffic
* Unusual HTTP requests

---

# 7. Network Security Policy for CoreTech Innovation

## Purpose

Protect company networks and information systems.

## Policy

* Use strong passwords.
* Enable Multi-Factor Authentication (MFA).
* Configure firewalls on all systems.
* Update operating systems regularly.
* Install antivirus software.
* Use VPN for remote access.
* Monitor network activity.
* Restrict unnecessary ports.
* Perform regular security audits.
* Train employees on cybersecurity awareness.

---

# Conclusion

Firewalls, IDS/IPS systems, VPNs, and packet analysis tools work together to protect networks from cyber threats. A well-defined security policy and continuous monitoring are essential for maintaining a secure network.

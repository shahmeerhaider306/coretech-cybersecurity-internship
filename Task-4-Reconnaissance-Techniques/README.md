Author: Shahmeer Haider
# Reconnaissance Techniques in Ethical Hacking

## Introduction

Reconnaissance is the information-gathering phase of ethical hacking. It helps security professionals understand a target's digital footprint before performing security assessments. Reconnaissance must always be conducted on legal and authorized targets.

---

# 1. Passive vs Active Reconnaissance

## Passive Reconnaissance

Passive reconnaissance involves collecting information about a target without directly interacting with its systems.

### Examples

* Google searches
* WHOIS lookup
* Social media research
* Public DNS records
* Shodan searches

### Advantages

* Difficult to detect
* No direct contact with target systems

---

## Active Reconnaissance

Active reconnaissance involves directly interacting with the target system to gather information.

### Examples

* Ping scans
* Port scanning
* DNS queries
* Network mapping

### Advantages

* More accurate and detailed information

### Disadvantages

* May be detected by security systems

---

# Comparison Table

| Passive Reconnaissance | Active Reconnaissance |
| ---------------------- | --------------------- |
| No direct interaction  | Direct interaction    |
| Hard to detect         | Easier to detect      |
| Uses public sources    | Uses network requests |
| Safer approach         | More detailed results |

---

# 2. WHOIS Lookup

WHOIS provides information about domain registration.

## Example Command

```bash
whois example.com
```

## Sample Information Obtained

* Domain Name
* Registrar
* Registration Date
* Expiration Date
* Name Servers

### Example Output

<img width="907" height="554" alt="image" src="https://github.com/user-attachments/assets/665c0381-811c-4c20-868a-1a644cc515e5" />

# 3. DNS Information Gathering Using nslookup

nslookup is used to query DNS records.

## Example Command

```bash
nslookup example.com
```

### Sample Output

<img width="444" height="364" alt="image" src="https://github.com/user-attachments/assets/39498757-8a9a-4c85-8bed-c7e50c2a346b" />

---

# 4. DNS Information Gathering Using dig

dig provides detailed DNS information.

## Example Command

```bash
dig example.com
```

### Sample Output

<img width="335" height="68" alt="image" src="https://github.com/user-attachments/assets/7f6d4642-65f8-4adc-9d36-baadb28c2f2c" />

---

# 5. Google Dorking

Google Dorking uses advanced search operators to find publicly available information.

## Example 1

```txt
site:example.com
```

<img width="1221" height="534" alt="image" src="https://github.com/user-attachments/assets/80e182cd-ee97-485a-982c-39f2826a210c" />

---

## Example 2

```txt
site:example.com filetype:pdf
```

Finds PDF documents.

---

## Example 3

```txt
intitle:"index of"
```

Finds publicly listed directories.

---

## Example 4

```txt
inurl:login
```

Searches pages containing "login" in the URL.

---

## Example 5

```txt
site:example.com contact
```

Finds contact-related pages.

---

# 6. Shodan Search Concepts

Shodan is a search engine that indexes internet-connected devices.

## Common Search Examples

### Web Servers

```txt
apache
```

<img width="1918" height="931" alt="image" src="https://github.com/user-attachments/assets/feda5ad0-c052-492c-8a1a-f8acb49ebbd8" />

---

### Webcam Search

```txt
webcam
```

<img width="1907" height="934" alt="image" src="https://github.com/user-attachments/assets/c92b12c5-2e35-4549-8716-d9fae2ab3fe7" />

---

### FTP Services

```txt
port:21
```

---

### HTTPS Services

```txt
port:443
```

---

### Country Filter

```txt
apache country:"US"
```

---

# 7. Legal and Ethical Considerations

Reconnaissance activities should only be performed on:

* Personal lab environments
* Authorized systems
* Educational targets
* Systems with explicit permission

Unauthorized scanning or information gathering may violate laws and organizational policies.

---

# Findings

The exercises demonstrated how publicly available information can reveal important details about domains, DNS infrastructure, and internet-connected services. Reconnaissance is an essential first step in cybersecurity assessments and helps identify potential attack surfaces.

---

# Conclusion

Passive and active reconnaissance techniques are fundamental skills in ethical hacking. WHOIS, nslookup, dig, Google Dorking, and Shodan help security professionals gather information while respecting legal and ethical boundaries.

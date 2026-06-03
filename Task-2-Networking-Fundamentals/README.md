Author: Shahmeer Haider
# Networking Fundamentals for Cybersecurity

# Introduction

Networking fundamentals are very important in cybersecurity because they help us understand how devices communicate and how attackers exploit networks. Understanding networking concepts helps cybersecurity professionals secure systems and detect attacks.

---

# 1. OSI Model

The OSI (Open Systems Interconnection) Model is a 7-layer framework used to understand how network communication works.

## OSI Model Layers

| Layer | Name               | Function                                               |
| ----- | ------------------ | ------------------------------------------------------ |
| 7     | Application Layer  | Provides services to users like web browsing and email |
| 6     | Presentation Layer | Translates and encrypts data                           |
| 5     | Session Layer      | Establishes and manages connections                    |
| 4     | Transport Layer    | Ensures reliable data delivery                         |
| 3     | Network Layer      | Handles routing and IP addressing                      |
| 2     | Data Link Layer    | Transfers data between devices on same network         |
| 1     | Physical Layer     | Sends raw bits through cables and hardware             |

## Simple OSI Diagram

<img width="560" height="516" alt="The 7 Layers of OSI" src="https://github.com/user-attachments/assets/0c71a827-ab77-4900-8913-436fcd414cc2" />

# 2. TCP/IP Model

The TCP/IP model is the practical networking model used on the internet.

## Layers of TCP/IP Model

| Layer                | Function                        |
| -------------------- | ------------------------------- |
| Application Layer    | User services like HTTP and FTP |
| Transport Layer      | Communication using TCP or UDP  |
| Internet Layer       | Routing and IP addressing       |
| Network Access Layer | Physical transmission of data   |

<img width="866" height="626" alt="TCP Diagram" src="https://github.com/user-attachments/assets/6d8fdc75-665f-4f4d-b581-c459e1391509" />

---

# 3. Common Network Protocols

## HTTP

HTTP (HyperText Transfer Protocol) is used for web communication.

## HTTPS

HTTPS is the secure version of HTTP using encryption.

## FTP

FTP (File Transfer Protocol) is used for transferring files.

## SSH

SSH (Secure Shell) is used for secure remote login and administration.

## DNS

DNS (Domain Name System) converts domain names into IP addresses.

## DHCP

DHCP (Dynamic Host Configuration Protocol) automatically assigns IP addresses to devices.

---

# 4. IP Addressing and Subnetting Basics

## IP Address

An IP address identifies a device on a network.

Example:

```txt
192.168.1.1
```

## Types of IP Addresses

* Private IP
* Public IP

## Subnetting

Subnetting divides a network into smaller networks for better management and security.

Example subnet mask:

```txt
255.255.255.0
```

---

# 5. Difference Between TCP and UDP

| TCP                  | UDP                          |
| -------------------- | ---------------------------- |
| Reliable             | Faster                       |
| Connection-oriented  | Connectionless               |
| Error checking       | No error checking            |
| Used in web browsing | Used in gaming and streaming |

---

# 6. Types of Network Attacks

## Man-in-the-Middle Attack

An attacker secretly intercepts communication between two users.

---

## DNS Spoofing

Attackers provide fake DNS responses to redirect users to malicious websites.

---

## ARP Poisoning

Attackers send fake ARP messages to connect their MAC address with another device's IP address.

---

# 7. Firewalls and Routers

## Firewall

A firewall monitors and filters incoming and outgoing network traffic to block unauthorized access.

### Firewall Diagram

<img width="800" height="400" alt="image" src="https://github.com/user-attachments/assets/c4f257da-4d38-4dab-9b87-c86bd887ecef" />

---

## Router

A router connects multiple networks and forwards data packets between them.

### Router Diagram

<img width="1168" height="590" alt="image" src="https://github.com/user-attachments/assets/4cc64d62-2825-423e-b0ca-c762ed46401b" />

---

# Conclusion

Networking fundamentals are essential for cybersecurity professionals. Understanding models, protocols, IP addressing, attacks, firewalls, and routers helps in protecting systems and securing communication networks.

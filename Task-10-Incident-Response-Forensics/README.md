# Incident Response and Digital Forensics

# Introduction

Incident response and digital forensics help organizations detect, investigate, respond to, and recover from cybersecurity incidents while preserving evidence for analysis.

---

# 1. Incident Response Lifecycle

## 1. Preparation

Preparation involves creating policies, training employees, maintaining backups, and deploying security tools before an incident occurs.

### Activities

* Create incident response plan
* Train security team
* Configure monitoring systems
* Maintain backups

---

## 2. Detection and Analysis

Identify suspicious activities using alerts, logs, and monitoring tools.

### Activities

* Monitor alerts
* Analyze logs
* Confirm security incident
* Assess impact

---

## 3. Containment

Contain the incident to prevent further damage.

### Activities

* Disconnect infected devices
* Block malicious IP addresses
* Disable compromised accounts

---

## 4. Eradication

Remove the root cause of the incident.

### Activities

* Remove malware
* Delete malicious files
* Patch vulnerabilities

---

## 5. Recovery

Restore affected systems safely.

### Activities

* Restore from backups
* Monitor systems
* Verify normal operation

---

## 6. Lessons Learned

Review the incident and improve future security.

### Activities

* Document findings
* Update policies
* Improve security controls

---

# 2. Incident Response Plan (Ransomware Scenario)

## Scenario

A ransomware attack encrypts company files and displays a ransom demand.

## Response Steps

1. Isolate infected computers.
2. Notify the incident response team.
3. Preserve logs and evidence.
4. Identify affected systems.
5. Remove ransomware.
6. Restore files from backups.
7. Reset compromised passwords.
8. Monitor systems after recovery.
9. Document the incident.
10. Conduct a lessons-learned meeting.

<img width="1889" height="414" alt="image" src="https://github.com/user-attachments/assets/f9159bc2-49ec-4b06-9cbf-994e5effcfea" />

---

# 3. Digital Forensics Basics

Digital forensics is the process of collecting, preserving, analyzing, and presenting digital evidence.

---

## Evidence Collection

Evidence should be collected without altering original data.

Examples:

* Hard drives
* USB devices
* System logs
* Memory dumps

---

## Chain of Custody

The chain of custody records who collected, handled, and analyzed digital evidence to ensure integrity.

---

## Disk Imaging

Disk imaging creates an exact bit-by-bit copy of a storage device for forensic analysis.

Benefits:

* Preserves original evidence
* Prevents accidental modification

---

# 4. Basic Digital Forensics Tools

## Autopsy

Autopsy is an open-source digital forensic platform used to examine disk images and recover evidence.

---

## FTK Imager

FTK Imager is used to create forensic disk images and preview digital evidence.

---

# 5. Log Analysis

Log analysis involves reviewing system, application, and security logs to detect suspicious activities.

Common logs include:

* Windows Event Logs
* Linux Syslog
* Web Server Logs
* Firewall Logs

---

# 6. SIEM Systems

Security Information and Event Management (SIEM) systems collect and analyze security logs from multiple devices.

Examples:

* Splunk
* IBM QRadar
* Microsoft Sentinel
* Elastic SIEM

<img width="1902" height="952" alt="image" src="https://github.com/user-attachments/assets/21f04f3d-7285-44b3-913c-21bb295b8d58" />

<img width="1551" height="863" alt="image" src="https://github.com/user-attachments/assets/fb5d52ae-adb5-42fc-85b3-eebc829d016d" />

<img width="789" height="526" alt="image" src="https://github.com/user-attachments/assets/ac875580-c902-4382-a804-c0aeeccce3c9" />


Benefits:

* Centralized monitoring
* Real-time alerts
* Incident investigation
* Compliance reporting

---

# 7. Post-Incident Report Template

## Incident Information

* Incident ID:
* Date:
* Reporter:
* Incident Type:

---

## Summary

Brief description of the incident.

---

## Timeline

* Detection Time
* Containment Time
* Recovery Time

---

## Affected Systems

List affected devices, servers, or applications.

---

## Root Cause

Describe the cause of the incident.

---

## Actions Taken

* Containment
* Eradication
* Recovery

---

## Recommendations

* Improve backups
* Strengthen endpoint protection
* Conduct employee awareness training
* Apply security patches
* Review security policies

---

# Conclusion

A well-defined incident response process and proper digital forensics techniques help organizations minimize damage, recover quickly, and improve future security. Documentation, evidence preservation, and continuous improvement are key components of effective cybersecurity incident management.

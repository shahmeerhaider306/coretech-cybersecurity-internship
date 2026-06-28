# Web Application Security Concepts

# Introduction

Web application security focuses on protecting websites and web applications from cyber attacks. Security professionals identify vulnerabilities and apply controls to protect user data and maintain secure communication.

---

# 1. OWASP Top 10 Vulnerabilities

The OWASP Top 10 is a list of the most critical web application security risks.

<img width="1904" height="855" alt="image" src="https://github.com/user-attachments/assets/e17deeb8-d9c6-4303-baa8-fc30858de5c6" />


## 1. Broken Access Control

Users can access resources or perform actions they should not be allowed to.

## 2. Cryptographic Failures

Sensitive information is exposed because of weak or incorrect encryption.

## 3. Injection

Attackers inject malicious commands or queries into an application (for example, SQL Injection).

## 4. Insecure Design

Security is not considered during application design, leading to weaknesses.

## 5. Security Misconfiguration

Default settings, unnecessary services, or incorrect configurations expose the application.

## 6. Vulnerable and Outdated Components

Using software with known security vulnerabilities.

## 7. Identification and Authentication Failures

Weak login systems allow unauthorized access.

## 8. Software and Data Integrity Failures

Applications trust unverified updates or insecure software components.

## 9. Security Logging and Monitoring Failures

Insufficient logging makes attacks difficult to detect.

## 10. Server-Side Request Forgery (SSRF)

An attacker tricks the server into making requests to unintended resources.

---

# 2. SQL Injection (SQLi)

## Concept

SQL Injection occurs when user input is incorrectly included in SQL queries, allowing attackers to manipulate the database.

## Example

```sql
SELECT * FROM users WHERE username='admin' AND password='password';
```

If input is not validated, an attacker may alter the query.

## Prevention

* Use parameterized queries (prepared statements).
* Validate and sanitize input.
* Apply the principle of least privilege for database accounts.
* Keep database software updated.

---

# 3. Cross-Site Scripting (XSS)

## Concept

XSS allows attackers to inject malicious scripts into web pages viewed by other users.

## Example

```html
<script>alert('XSS')</script>
```

## Prevention

* Validate and sanitize user input.
* Encode output before displaying it.
* Use Content Security Policy (CSP).
* Set cookies with appropriate security flags.

---

# 4. Cross-Site Request Forgery (CSRF)

## Concept

CSRF tricks an authenticated user into performing unwanted actions on a website.

## Prevention

* Use CSRF tokens.
* Verify the Origin or Referer header where appropriate.
* Require re-authentication for sensitive actions.

---

# 5. Broken Authentication and Session Management

## Concept

Weak authentication or poor session handling can allow attackers to hijack accounts.

## Prevention

* Use strong passwords.
* Enable Multi-Factor Authentication (MFA).
* Set secure session timeouts.
* Use secure, random session IDs.

---

# 6. Security Misconfiguration

## Concept

Improper server or application settings create security risks.

## Examples

* Default passwords
* Debug mode enabled in production
* Unnecessary open services
* Missing security updates

## Prevention

* Change default settings.
* Disable unnecessary services.
* Apply security patches.
* Regularly review configurations.

---

# 7. HTTPS and Web Security

HTTPS protects web traffic by encrypting communication between the browser and the web server using TLS.

## Benefits

* Encrypts transmitted data.
* Protects against eavesdropping.
* Helps prevent data tampering.
* Authenticates the server using digital certificates.

---

# 8. Practice Platforms

Safe platforms for learning web application security include:

* DVWA (Damn Vulnerable Web Application)
* TryHackMe
* Hack The Box

These platforms are designed for legal and educational practice.

<img width="1915" height="750" alt="image" src="https://github.com/user-attachments/assets/746fda3d-1725-4a72-a70f-104d80f015dc" />

<img width="1920" height="881" alt="image" src="https://github.com/user-attachments/assets/251ddd8d-332b-4049-be99-ab386dea172e" />

<img width="1905" height="952" alt="image" src="https://github.com/user-attachments/assets/6abf51d5-81b6-4d0c-94f9-664a2af73b24" />


---

# Conclusion

Understanding web application vulnerabilities helps developers and security professionals build safer applications. Learning the OWASP Top 10 and practicing on legal training platforms improves the ability to identify risks and implement effective security controls.

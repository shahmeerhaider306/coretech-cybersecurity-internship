# Password Security and Cryptography

# Introduction

Password security and cryptography are essential parts of cybersecurity. They protect sensitive information by using encryption, hashing, and secure authentication methods.

---

# 1. Symmetric vs Asymmetric Encryption

## Symmetric Encryption

Symmetric encryption uses the **same key** for both encryption and decryption.

### Examples

* AES
* DES

### Advantages

* Fast
* Efficient for large amounts of data

### Disadvantages

* Secure key sharing is required.

---

## Asymmetric Encryption

Asymmetric encryption uses **two keys**:

* Public Key
* Private Key

### Examples

* RSA
* ECC

### Advantages

* More secure for communication
* Supports digital signatures

### Disadvantages

* Slower than symmetric encryption

---

# Comparison

| Symmetric | Asymmetric |
| --------- | ---------- |
| One key   | Two keys   |
| Faster    | Slower     |
| AES, DES  | RSA, ECC   |

---

# 2. Hashing Algorithms

Hashing converts data into a fixed-length value.

## MD5

Produces a 128-bit hash.

Example:

```text
5f4dcc3b5aa765d61d8327deb882cf99
```

### Why MD5 is Insecure

* Vulnerable to collision attacks
* Fast to brute-force
* Not recommended for passwords

---

## SHA-1

Produces a 160-bit hash.

Also considered insecure because collision attacks have been demonstrated.

---

## SHA-256

Produces a 256-bit hash.

More secure and commonly used today.

---

# 3. Password Hashing in Python

Example using hashlib:



<img width="703" height="155" alt="image" src="https://github.com/user-attachments/assets/e3272532-062a-4958-8b9b-5e2acbb07460" />

Output:

<img width="626" height="44" alt="image" src="https://github.com/user-attachments/assets/b029316f-62dc-4879-a997-60f12407fe1f" />


This converts the password into a SHA-256 hash.

---

# 4. Salting

A salt is random data added to a password before hashing.

Example:

Password:

```text
Password123
```

Salt:

```text
aB7#x9
```

Combined:

```text
Password123aB7#x9
```

<img width="1665" height="907" alt="image" src="https://github.com/user-attachments/assets/7880470c-c14b-437d-a275-67121ef5b454" />


## Importance of Salting

* Prevents rainbow table attacks.
* Makes identical passwords produce different hashes.
* Increases password security.

---

# 5. Password Cracking Concepts

Password recovery tools help security professionals test password strength in authorized environments.

Common tools include:

* Hashcat
* John the Ripper

These tools should only be used on systems you own or have permission to test.

<img width="1911" height="953" alt="image" src="https://github.com/user-attachments/assets/7557093e-22fe-4bbf-873b-559da7c45351" />

<img width="1904" height="939" alt="image" src="https://github.com/user-attachments/assets/37468c21-95e3-4081-9a03-08854e5a1f38" />


---

# 6. SSL/TLS

SSL/TLS encrypts communication between a client and a server.

Benefits:

* Encrypts transmitted data.
* Prevents eavesdropping.
* Protects user privacy.
* Ensures secure communication.

---

# 7. How Digital Certificates Work

A digital certificate:

* Verifies a website's identity.
* Contains the public key.
* Is issued by a trusted Certificate Authority (CA).
* Enables secure HTTPS communication.

---

# 8. Password Security Best Practices for CoreTech Innovation

* Use passwords with at least 12 characters.
* Include uppercase, lowercase, numbers, and symbols.
* Enable Multi-Factor Authentication (MFA).
* Never reuse passwords across multiple accounts.
* Store passwords using strong hashing algorithms such as SHA-256 or bcrypt.
* Apply salting before hashing passwords.
* Change passwords if compromise is suspected.
* Use a trusted password manager.
* Keep systems and applications updated.
* Train employees on password security awareness.

---

# Conclusion

Strong password practices and modern cryptography help protect systems from unauthorized access. Organizations should use secure hashing algorithms, salting, encryption, SSL/TLS, and strong password policies to improve cybersecurity.

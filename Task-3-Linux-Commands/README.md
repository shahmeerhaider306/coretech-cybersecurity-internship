Author: Shahmeer Haider
# Linux Commands for Cybersecurity

# Introduction

Linux is widely used in cybersecurity because it provides powerful command-line tools for networking, system administration, penetration testing, and security analysis. Understanding Linux commands is essential for cybersecurity professionals.

---

# 1. File System Navigation Commands

## ls

Used to list files and folders.

### Command

```bash
ls
```

### Example Output

```txt
Documents Downloads Pictures
```

---

<img width="241" height="49" alt="image" src="https://github.com/user-attachments/assets/0f1e9433-8ec4-48c7-a96d-85f97af86fa0" />

## cd

Used to change directory.

### Command

```bash
cd Documents
```

---

<img width="198" height="39" alt="image" src="https://github.com/user-attachments/assets/c3e9be5f-f85b-445f-b0cf-1c8a4cb64653" />


## pwd

Shows current directory path.

### Command

```bash
pwd
```

### Example Output

```txt
/home/user/Documents
```

---

<img width="193" height="56" alt="image" src="https://github.com/user-attachments/assets/b1b16c09-92d9-4382-bcd8-a0fc2c336498" />

## mkdir

Creates a new folder.

### Command

```bash
mkdir cybersecurity
```

---

<img width="282" height="48" alt="image" src="https://github.com/user-attachments/assets/4de204b1-f9f3-4b6c-bf37-575ad55f2e83" />

## rm

Removes files or folders.

### Command

```bash
rm file.txt
```

---


<img width="194" height="34" alt="image" src="https://github.com/user-attachments/assets/335b45a6-46d5-4b69-a6c3-29210765a97c" />


# 2. File Permission Commands

## chmod

Changes file permissions.

### Command

```bash
chmod 755 file.txt
```

---

<img width="235" height="37" alt="image" src="https://github.com/user-attachments/assets/4246001a-f22d-426c-9462-9b1805d69742" />


## chown

Changes file owner.

### Command

```bash
chown user file.txt
```

---

<img width="244" height="45" alt="image" src="https://github.com/user-attachments/assets/7c89096b-7687-4ec9-8b9a-30efbed0543a" />


# 3. User Management Commands

## adduser

Creates a new user.

### Command

```bash
adduser ali
```

---

<img width="273" height="39" alt="image" src="https://github.com/user-attachments/assets/c4c7eb55-e9f3-42d6-b035-1d3b17ef9d09" />


## passwd

Changes user password.

### Command

```bash
passwd ali
```

---

<img width="204" height="41" alt="image" src="https://github.com/user-attachments/assets/8b70fe85-c99b-40ab-a302-14b5a3e4e91e" />


# 4. Networking Commands

## ifconfig

Displays network configuration.

### Command

```bash
ifconfig
```

---

<img width="159" height="47" alt="image" src="https://github.com/user-attachments/assets/9bce4f0c-3b97-4f16-b04f-d92fd7a1d3a9" />


## ping

Checks connectivity between devices.

### Command

```bash
ping google.com
```

---

<img width="210" height="53" alt="image" src="https://github.com/user-attachments/assets/7ce44360-66ff-4b6f-8427-17b7703b1155" />


## netstat

Shows network connections and ports.

### Command

```bash
netstat -a
```

---

<img width="168" height="39" alt="image" src="https://github.com/user-attachments/assets/c2c552ac-dfe3-41d3-ac6a-d48439395ef0" />


## nmap

Used for network scanning.

### Command

```bash
nmap 192.168.1.1
```

---

<img width="223" height="40" alt="image" src="https://github.com/user-attachments/assets/5b7aa360-695b-46d8-b001-8442261b0e83" />


# 5. Process Management Commands

## ps

Displays running processes.

### Command

```bash
ps
```

---

<img width="87" height="39" alt="image" src="https://github.com/user-attachments/assets/1995b247-0daf-44be-a88c-024550e1c719" />


## kill

Terminates a process.

### Command

```bash
kill 1234
```

---

<img width="166" height="45" alt="image" src="https://github.com/user-attachments/assets/f968473c-23b5-4609-b922-34ae1020b3e5" />


## top

Shows real-time system processes.

### Command

```bash
top
```

---

<img width="136" height="45" alt="image" src="https://github.com/user-attachments/assets/500015b1-9f15-4413-bd0b-b6692959b954" />


# 6. Package Management Commands

## apt-get

Installs or updates packages.

### Command

```bash
apt-get update
```

---

<img width="212" height="55" alt="image" src="https://github.com/user-attachments/assets/44ba00a7-1ce8-465b-933f-ba01b5214d7a" />


## sudo

Runs commands with administrator privileges.

### Command

```bash
sudo apt-get install nmap
```

---

<img width="296" height="45" alt="image" src="https://github.com/user-attachments/assets/e2894ccd-ee3a-4939-b5ae-4423c010549a" />


# Additional Linux Commands

## touch

Creates a new empty file.

```bash
touch notes.txt
```

---

## cp

Copies files.

```bash
cp file1.txt file2.txt
```

---

## mv

Moves or renames files.

```bash
mv old.txt new.txt
```

---

## cat

Displays file contents.

```bash
cat notes.txt
```

---

## clear

Clears terminal screen.

```bash
clear
```

---

## whoami

Shows current logged-in user.

```bash
whoami
```

---

## history

Displays previously used commands.

```bash
history
```

---

## uname

Shows system information.

```bash
uname -a
```

---

## df

Displays disk space usage.

```bash
df -h
```

---

## free

Shows memory usage.

```bash
free -m
```

---

# Importance of Linux in Cybersecurity

Linux provides flexibility, security tools, and powerful networking capabilities. Many cybersecurity tools such as Kali Linux, Nmap, and Wireshark are Linux-based.

---

# Conclusion

Learning Linux commands is an important step in cybersecurity. These commands help professionals manage systems, analyze networks, monitor processes, and secure systems effectively.

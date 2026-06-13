# Linux Task 02: Users, Groups & File Permissions

**Date:** June 2026
**Name:** Sayali Kute

---

## 🔍 Task Objectives

The purpose of this task was to understand Linux user management, groups, file ownership, and file permissions. These concepts are essential for Linux security, system administration, and cybersecurity.

---

# Part A: Understanding Users

## Commands Used

```bash
whoami
id
cat /etc/passwd
```

## Findings

### Current Username

The current logged-in user is:

```text
sayali
```

### What is UID?

UID (User Identifier) is a unique numerical value assigned to each Linux user account.

### What is GID?

GID (Group Identifier) is a unique numerical value assigned to a Linux group.

### What information does /etc/passwd contain?

The /etc/passwd file contains user account information including username, UID, GID, home directory, login shell, and account details.

---

# Part B: Create Users & Groups

## Groups Created

```text
interns
cyberteam
```

## Users Created

```text
student1
student2
student3
```

## Commands Used

```bash
sudo groupadd interns
sudo groupadd cyberteam

sudo useradd student1
sudo useradd student2
sudo useradd student3

sudo usermod -aG interns student1
sudo usermod -aG interns student2
sudo usermod -aG cyberteam student3
```

## Verification Commands

```bash
groups
id student1
id student2
id student3
```

Users were successfully added to their respective groups.

---

# Part C: File Ownership

## Directory Created

```text
CyberSecurity_Project
```

## Files Created

```text
report.txt
notes.txt
credentials.txt
```

## Commands Used

```bash
mkdir CyberSecurity_Project
cd CyberSecurity_Project

touch report.txt
touch notes.txt
touch credentials.txt

ls -l
sudo chown student1 report.txt
ls -l
```

## Ownership Change

| Item           | Value                          |
| -------------- | ------------------------------ |
| Original Owner | sayali                         |
| New Owner      | student1                       |
| Command Used   | sudo chown student1 report.txt |

The ownership of report.txt was successfully transferred.

---

# Part D: File Permissions

## File Created

```text
security_policy.txt
```

## Commands Used

### Read Only

```bash
chmod 444 security_policy.txt
```

### Read & Write

```bash
chmod 664 security_policy.txt
```

### Full Access

```bash
chmod 777 security_policy.txt
```

## Purpose

The chmod command is used to modify file permissions and control user access.

---

# Part E: Permission Analysis

| Permission | Owner | Group | Others | Use Case                                    |
| ---------- | ----- | ----- | ------ | ------------------------------------------- |
| 755        | rwx   | r-x   | r-x    | Executable scripts and directories          |
| 644        | rw-   | r--   | r--    | Documents and configuration files           |
| 777        | rwx   | rwx   | rwx    | Full access for all users (not recommended) |
| 600        | rw-   | ---   | ---    | Password files and private data             |
| 700        | rwx   | ---   | ---    | Private directories and scripts             |

---

# Part F: Security Challenge

| File                | Recommended Permission | Reason                            |
| ------------------- | ---------------------- | --------------------------------- |
| password_backup.txt | 600                    | Contains sensitive credentials    |
| public_notice.txt   | 644                    | Publicly readable document        |
| system_log.txt      | 640                    | Accessible to administrators only |
| personal_notes.txt  | 600                    | Private personal information      |

---

# Part G: Linux Security Research

## Why are file permissions important?

File permissions control access to files and directories, helping protect sensitive information and maintain system security.

## What happens if sensitive files are given 777 permissions?

Any user can read, modify, or delete the files, creating serious security risks and increasing the possibility of unauthorized access.

## What is the Principle of Least Privilege?

The Principle of Least Privilege states that users should only be granted the minimum permissions necessary to perform their tasks.

## Why do organizations restrict user access?

Organizations restrict access to protect confidential information, prevent accidental modifications, reduce insider threats, and improve overall security.

---

# Screenshots Included

The repository contains screenshots of:

* User Information Commands
* User and Group Creation
* Group Verification
* File Ownership Changes
* File Permission Modifications
* Permission Analysis Activities

---

# Learning Outcome

Through this task, I learned:

* Linux user management
* Group administration
* File ownership concepts
* chmod and chown commands
* Linux permission models
* Principle of Least Privilege
* Linux security best practices

---

# Conclusion

This task provided hands-on experience with Linux users, groups, file ownership, and permissions. Understanding these concepts is essential for system administration and cybersecurity because improper permissions can lead to security vulnerabilities and unauthorized access.

---

**Submitted as part of the White Band Associates Cyber Security Summer Internship Program.**

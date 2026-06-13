# Linux Task 01: Linux Environment Setup & Essential Commands

**Date:** June 12, 2026
**Name:** Sayali Kute

---

## 🔍 Task Objectives

The purpose of this task was to become familiar with the Linux operating system, terminal usage, navigation, file management, and basic system administration commands. Linux is one of the most important operating systems used in Cyber Security, Ethical Hacking, Cloud Computing, and Server Administration.

---

# Part A: Linux Installation & Verification

## Operating System Used

**Kali Linux**

## Verification

The following screenshots have been included in the repository:

* Linux Desktop Environment
* Terminal Window
* System Information

These screenshots confirm that Kali Linux was successfully installed and configured in a virtual machine environment.

---

# Part B: Basic Navigation Commands

The following Linux commands were executed using the terminal.

| Command  | Purpose                                                          |
| -------- | ---------------------------------------------------------------- |
| pwd      | Displays the current working directory                           |
| ls       | Lists files and directories                                      |
| ls -la   | Lists all files including hidden files with detailed information |
| cd       | Changes the current directory                                    |
| clear    | Clears the terminal screen                                       |
| history  | Displays previously executed commands                            |
| whoami   | Shows the currently logged-in user                               |
| hostname | Displays the system hostname                                     |

## Commands Executed

```bash
pwd
ls
ls -la
cd
clear
history
whoami
hostname
```

### Results

* Current User: **sayali**
* Hostname: **kali**
* Home Directory: **/home/sayali**

Screenshots of command execution have been included in the Screenshots folder.

---

# Part C: Directory Management

A directory structure named **CyberSecurity_Lab** was created.

## Commands Used

```bash
mkdir CyberSecurity_Lab
cd CyberSecurity_Lab
mkdir Networking Linux CyberSecurity EthicalHacking Reports
tree
```

## Directory Structure

```text
CyberSecurity_Lab
│
├── Networking
├── Linux
├── CyberSecurity
├── EthicalHacking
└── Reports
```

The directory structure was successfully created and verified using the tree command.

Screenshots have been included in the Screenshots folder.

---

# Part D: File Management

Several file management operations were performed inside the Networking directory.

## Files Created

```text
notes.txt
commands.txt
report.txt
```

## Commands Used

### Create Files

```bash
touch notes.txt
touch commands.txt
touch report.txt
```

### Copy Files

```bash
cp notes.txt notes_copy.txt
```

### Rename Files

```bash
mv commands.txt linux_commands.txt
```

### Move Files

```bash
mv report.txt ../Reports/
```

### Delete Files

```bash
rm notes_copy.txt
```

## Purpose of Commands

| Command | Purpose                |
| ------- | ---------------------- |
| touch   | Creates a new file     |
| cp      | Copies files           |
| mv      | Moves or renames files |
| rm      | Deletes files          |

Screenshots of file creation, copying, moving, renaming, and deletion have been included.

---

# Part E: System Information Collection

The following commands were executed to collect system information.

## Commands Used

```bash
uname -a
hostname
whoami
date
uptime
pwd
```

## Collected Information

| Item              | Value                    |
| ----------------- | ------------------------ |
| Username          | sayali                   |
| Hostname          | kali                     |
| Current Directory | /home/sayali             |
| Operating System  | Kali Linux               |
| Kernel Version    | Linux 6.18.12+kali-amd64 |
| Date and Time     | Captured in screenshot   |
| System Uptime     | Captured in screenshot   |

### uname -a Output

```text
Linux kali 6.18.12+kali-amd64 #1 SMP PREEMPT_DYNAMIC Kali 6.18.12-1kali1 x86_64 GNU/Linux
```

Screenshots have been included in the repository.

---

# Part F: Linux Research Activity

## What is Linux?

Linux is a free and open-source operating system based on the Linux kernel. It is widely used in servers, cloud computing, embedded systems, and cybersecurity environments because of its stability, security, and flexibility.

---

## Why is Linux Important in Cyber Security?

Linux is important in Cyber Security because most security tools, servers, and penetration-testing environments run on Linux. It provides powerful command-line utilities, scripting capabilities, and better control over system resources.

---

## Difference Between Linux and Windows

| Linux                 | Windows                             |
| --------------------- | ----------------------------------- |
| Open Source           | Proprietary                         |
| Free to Use           | Licensed Software                   |
| Highly Customizable   | Limited Customization               |
| Command-Line Friendly | GUI Focused                         |
| Common in Servers     | Common in Personal Computers        |
| More Secure           | More Frequently Targeted by Malware |

---

## What is a Linux Distribution?

A Linux Distribution (Distro) is a version of Linux that includes the Linux kernel along with software packages, desktop environments, and utilities. Examples include Ubuntu, Kali Linux, Debian, Fedora, and Parrot OS.

---

## Why Do Ethical Hackers Prefer Linux?

Ethical hackers prefer Linux because it offers powerful security tools, flexibility, scripting support, and complete control over the operating system. Most penetration-testing and cybersecurity tools are designed to run on Linux environments.

---

# Screenshots Included

The repository contains screenshots of:

* Linux Desktop Environment
* Terminal Window
* Navigation Commands
* Directory Structure Creation
* File Management Operations
* System Information Collection
* Linux Command Outputs

---

# Learning Outcome

Through this task, I gained practical experience with:

* Linux installation and setup
* Linux terminal navigation
* File and directory management
* System information gathering
* Linux command-line usage
* Basic Linux administration
* Cybersecurity-related Linux concepts

---

# Conclusion

This task helped me understand the fundamentals of Linux and its importance in Cyber Security. I learned how to navigate the Linux file system, manage files and directories, collect system information, and use essential Linux commands. These skills form the foundation for cybersecurity, ethical hacking, server management, and cloud computing.

---

**Submitted as part of the White Band Associates Cyber Security Summer Internship Program.**

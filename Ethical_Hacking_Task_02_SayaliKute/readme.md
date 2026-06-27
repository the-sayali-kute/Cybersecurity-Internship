# Network Scanning Task 02: Nmap Installation, Port Scanning & OS Detection

**Date:** June 27, 2026
**Name:** Sayali Kute

---

# 🔍 Task Objectives

* Install and verify Nmap on Windows.
* Perform a basic scan on the local machine.
* Identify open TCP ports and running services.
* Detect the operating system of the target.
* Understand the importance of network reconnaissance in cybersecurity.

---

# Part A: Nmap Installation Verification

## Command Used

```bash
nmap --version
```

### Installation Details

| Parameter             | Value      |
| --------------------- | ---------- |
| Nmap Version          | 7.99       |
| Platform              | Windows    |
| Packet Capture Driver | Npcap 1.83 |
| IPv6 Support          | Yes        |

### Observation

The installation was successful. Nmap version **7.99** and Npcap were installed correctly, allowing the system to perform network scanning and reconnaissance tasks.

---

# Part B: Localhost Scan

## Command Used

```bash
nmap localhost
```

### Scan Results

| Port | Protocol | State | Service            |
| ---- | -------- | ----- | ------------------ |
| 135  | TCP      | Open  | MSRPC              |
| 445  | TCP      | Open  | Microsoft-DS (SMB) |

### Scan Summary

| Item          | Result                |
| ------------- | --------------------- |
| Target        | localhost (127.0.0.1) |
| Host Status   | Up                    |
| Open Ports    | 2                     |
| Closed Ports  | 998                   |
| Scan Duration | 0.80 Seconds          |

### Observation

The localhost scan identified **two open TCP ports**. Port **135** is used by Microsoft Remote Procedure Call (MSRPC), while Port **445** is used by Microsoft Directory Services (SMB). The remaining scanned ports were closed.

---

# Part C: Service Version Detection

## Command Used

```bash
nmap -sV localhost
```

### Results

| Port | Service      | Version              |
| ---- | ------------ | -------------------- |
| 135  | MSRPC        | Version Not Detected |
| 445  | Microsoft-DS | Version Not Detected |

### Observation

The scan successfully detected the running services but could not determine the exact software versions. This is common on Windows systems because some services do not expose version information for security reasons.

---

# Part D: Operating System Detection

## Command Used

```bash
nmap -O localhost
```

### Results

| Parameter        | Value                     |
| ---------------- | ------------------------- |
| Device Type      | General Purpose           |
| Operating System | Microsoft Windows 11      |
| OS Details       | Microsoft Windows 11 23H2 |
| Network Distance | 0 Hops                    |

### Observation

The operating system detection scan correctly identified the local machine as **Microsoft Windows 11 (23H2)**. Since the scan was performed on the local system, the network distance was reported as **0 hops**.

---

# Questions & Answers

## 1. Which services are currently running?

The scan detected the following services:

* Microsoft Remote Procedure Call (MSRPC) – Port **135**
* Microsoft Directory Services (SMB) – Port **445**

---

## 2. Are all open ports necessary?

Not always. Some ports are required for normal operating system functions, while unnecessary open ports should be disabled because they increase the attack surface and may expose the system to security risks.

---

## 3. Which services could become security risks if misconfigured?

Examples include:

* SMB (Microsoft-DS)
* Remote Desktop Protocol (RDP)
* HTTP
* HTTPS
* FTP
* SSH
* DNS

---

## 4. Which port would you disable if it wasn't required?

If file and printer sharing were not needed, **Port 445 (SMB)** should be disabled because it is commonly targeted by malware, ransomware, and unauthorized network access.

---

# Screenshot Evidence

The repository includes the following screenshots:

* Nmap Installation Verification (`nmap --version`)
* Localhost Scan (`nmap localhost`)
* Service Version Detection (`nmap -sV localhost`)
* Operating System Detection (`nmap -O localhost`)

All screenshots are available in the **Screenshots** folder.

---

# Conclusion

This task provided practical experience with the Nmap network scanning tool. I learned how to install and verify Nmap, perform basic port scanning, identify running network services, and detect the operating system of a target machine. The activity demonstrated that open ports represent potential entry points into a system and should be regularly monitored to minimize security risks. I also understood the importance of reconnaissance as the first phase of penetration testing and cybersecurity assessments. This task strengthened my understanding of network scanning techniques and improved my hands-on skills with one of the most widely used security tools.

---

**Submitted as part of the White Band Association Cyber Security Summer Internship Program.**

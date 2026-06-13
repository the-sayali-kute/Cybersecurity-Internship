# Linux Task 03: Process Management, System Monitoring & Basic Shell Scripting

**Date:** June 2026
**Name:** Sayali Kute

---

# 🔍 Task Objectives

The purpose of this task was to understand Linux process management, system monitoring, service monitoring, and shell scripting. These skills are essential for Linux Administrators, SOC Analysts, and Cyber Security Professionals.

---

# Part A: Process Monitoring

## Commands Used

```bash
ps
ps aux
top
htop
```

## What is a Process?

A process is a running instance of a program executing on the operating system.

## What is a PID?

PID (Process ID) is a unique identifier assigned to each running process.

## Process Monitoring

The commands ps, ps aux, top, and htop were used to monitor running processes, CPU usage, memory usage, and system activity.

Screenshots of all commands are included in the Screenshots folder.

---

# Part B: Process Management

## Commands Used

```bash
sleep 300

ps aux | grep sleep

kill PID

kill -9 PID
```

## Activity Performed

A sleep process was started and located using process monitoring commands.

The process was terminated using both:

```bash
kill PID
```

and

```bash
kill -9 PID
```

This demonstrated how Linux manages and terminates running processes.

---

# Part C: System Monitoring

## Commands Used

```bash
free -h
df -h
uptime
uname -a
```

## System Information

| Item                 | Value                         |
| -------------------- | ----------------------------- |
| Total RAM            | 1.9 GiB                       |
| Available RAM        | 1.2 GiB                       |
| Disk Usage           | 19 GB Total, 18 GB Used       |
| Available Disk Space | 168 MB                        |
| System Uptime        | 1 Hour 27 Minutes             |
| Kernel Version       | Linux kali 6.18.12+kali-amd64 |

---

# Part D: Service Monitoring

## Commands Used

```bash
systemctl status ssh

systemctl status NetworkManager
```

## What is a Service?

A service is a background process that performs specific tasks for the operating system.

## Why are Services Important?

Services provide critical functionality such as networking, remote access, logging, and system management.

## Impact of a Stopped Service

If a service stops running, the associated functionality becomes unavailable and may affect system operations.

---

# Part E: Shell Scripting

## Script Name

system_report.sh

## Purpose

The script automatically generates a system information report displaying:

* Current User
* Hostname
* Date and Time
* Current Directory
* Available Memory
* Disk Usage

## Commands Used

```bash
chmod +x system_report.sh

./system_report.sh
```

The script was successfully executed and verified.

---

# Part F: Security Monitoring Research

## netstat

Displays network connections and listening ports.

### Security Use Case

Used to identify suspicious network activity.

---

## ss

Displays socket and network statistics.

### Security Use Case

Used to monitor active network connections.

---

## who

Displays currently logged-in users.

### Security Use Case

Used to identify active user sessions.

---

## w

Displays logged-in users and their activities.

### Security Use Case

Used to monitor user behavior and activity.

---

## last

Displays login history.

### Security Use Case

Used to investigate suspicious login attempts.

---

# Part G: Mini SOC Activity

If a Linux system is running slowly, I would use top or htop to identify resource-heavy processes.

To determine whether a process is suspicious, I would examine:

* Process name
* PID
* CPU usage
* Memory usage
* Executable path
* Process owner

Before terminating a process, I would collect information such as:

* PID
* Process name
* User account
* CPU usage
* Memory usage
* Associated services

This information helps prevent accidental termination of legitimate processes.

---

# Screenshots Included

The repository contains screenshots of:

* Process Monitoring Commands
* Process Management Activity
* System Monitoring Commands
* Service Monitoring
* Shell Script Creation
* Shell Script Execution

---

# Learning Outcome

Through this task, I learned:

* Linux process management
* Process monitoring techniques
* System resource monitoring
* Service monitoring
* Shell scripting basics
* Security monitoring commands
* SOC analyst fundamentals

---

# Conclusion

This task provided practical experience with Linux process management, system monitoring, service monitoring, and shell scripting. Understanding these concepts is essential for Linux administration, cybersecurity operations, incident response, and security monitoring.

---

**Submitted as part of the White Band Associates Cyber Security Summer Internship Program.**

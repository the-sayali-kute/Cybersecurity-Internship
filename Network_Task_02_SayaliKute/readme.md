# Networking Task 02: Network Devices & IP Addressing

**Date:** June 4, 2026
**Name:** Sayali Kute

---

## 🔍 Task Objectives

* Understand common network devices and their functions.
* Learn IP address classification and identify public and private IP addresses.
* Analyze my own network configuration.
* Understand how DNS and network communication work.
* Perform practical networking commands and document the results.

---

## Part A: Network Devices Research

### Router

**Purpose:** Connects different networks and forwards data between them.

**How It Works:** Uses IP addresses to determine the best path for data packets.

**Real-World Usage:** Home Wi-Fi routers connect devices to the internet.

---

### Switch

**Purpose:** Connects multiple devices within the same local network.

**How It Works:** Uses MAC addresses to send data directly to the intended device.

**Real-World Usage:** Used in offices, schools, and organizations.

---

### Hub

**Purpose:** Connects multiple devices in a network.

**How It Works:** Broadcasts incoming data to all connected devices.

**Real-World Usage:** Older networks before switches became common.

---

### Access Point

**Purpose:** Provides wireless connectivity to devices.

**How It Works:** Extends a wired network into a wireless network.

**Real-World Usage:** Wi-Fi hotspots in homes, colleges, and offices.

---

### Firewall

**Purpose:** Protects networks from unauthorized access and cyber threats.

**How It Works:** Monitors and filters incoming and outgoing network traffic.

**Real-World Usage:** Windows Firewall and enterprise security systems.

---

### Modem

**Purpose:** Connects a network to an Internet Service Provider (ISP).

**How It Works:** Converts digital signals into a form suitable for internet transmission.

**Real-World Usage:** Broadband and fiber internet connections.

---

## Part B: IP Address Classification

| IP Address    | Category | Reason                                                          |
| ------------- | -------- | --------------------------------------------------------------- |
| 192.168.1.10  | Private  | Falls within the private IP range 192.168.0.0 – 192.168.255.255 |
| 10.0.0.5      | Private  | Falls within the private IP range 10.0.0.0 – 10.255.255.255     |
| 172.16.5.20   | Private  | Falls within the private IP range 172.16.0.0 – 172.31.255.255   |
| 8.8.8.8       | Public   | Google's public DNS server                                      |
| 1.1.1.1       | Public   | Cloudflare's public DNS server                                  |
| 192.168.100.1 | Private  | Falls within the private IP range 192.168.0.0 – 192.168.255.255 |

---

## Part C: Understanding My Network

### System Information

| Parameter       | Value        |
| --------------- | ------------ |
| IPv4 Address    | 10.36.29.107 |
| Default Gateway | 10.36.29.72  |
| DNS Server      | 10.36.29.72  |

### Questions & Answers

#### Which IP range does your device belong to?

My device belongs to the **10.x.x.x private IP range**.

#### Is it Public or Private?

It is a **Private IP Address** because it falls within the reserved private IP range of **10.0.0.0 – 10.255.255.255**.

#### What role does your router play in your network?

The router connects my local network to the internet and forwards data packets between devices and external networks.

#### What would happen if the DNS server stopped working?

Domain names such as google.com would not resolve into IP addresses, making websites inaccessible unless users entered the IP address directly.

---

## Part D: Network Communication Flow

### Communication Process

Your Device
↓
Router
↓
DNS Server
↓
Google Server
↓
Response Back to Device

### Explanation

**Step 1:** The user enters [www.google.com](http://www.google.com) into a web browser.

**Step 2:** The request is sent to the router, which forwards it to the DNS server.

**Step 3:** The DNS server translates the domain name into an IP address.

**Step 4:** The browser sends a request to Google's server using the IP address.

**Step 5:** Google's server processes the request and sends the response back.

**Step 6:** The webpage is displayed on the user's device.

A network communication diagram is included in the repository.

---

## Part E: Practical Command Exercise

### Commands Used

```bash
ipconfig /all
nslookup google.com
ping google.com
```

### DNS Lookup Results

The DNS server successfully resolved **google.com** and returned multiple IPv4 and IPv6 addresses.

Example IPv4 Address:

```text
142.250.143.101
```

### Ping Test Results

* Ping was successful.
* DNS resolution completed successfully.
* Communication with Google servers was established.

### Questions & Answers

#### What IP address did DNS return for Google?

DNS returned multiple IPv4 and IPv6 addresses. One of the IPv4 addresses returned was:

```text
142.250.143.101
```

#### Was the ping successful?

Yes, the ping was successful.

#### Why is DNS important before communication begins?

DNS converts human-readable domain names into IP addresses, allowing devices to locate and communicate with servers on the internet.

---

## Screenshot Evidence

The repository contains screenshots of:

* ipconfig /all output
* nslookup google.com output
* ping google.com output
* Network communication diagram

All screenshots are available in the **Screenshots** folder.

---

## Conclusion

This task helped me understand the functions of various network devices, IP address classification, DNS resolution, and network communication processes. I also gained practical experience using networking tools such as ipconfig, nslookup, and ping to analyze network connectivity and configuration.

---

**Submitted as part of the White Band Associates Cyber Security Summer Internship Program.**

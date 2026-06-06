# Networking Task 01: Understanding Your Network Environment

**Date:** June 2, 2026
**Name:** Sayali Kute


## 🔍 Task Objectives

* Identify and document network configuration details of my system.
* Understand basic networking concepts.
* Create a simple network diagram.
* Test network connectivity using ping and traceroute commands.


## Part A: Network Information

### System Information

| Parameter              | Value             |
| ---------------------- | ----------------- |
| Hostname (Device Name) | SAYALI            |
| IPv4 Address           | 10.36.29.107      |
| MAC Address            | XX-BA-EF-8E-XX-XX |
| Default Gateway        | 10.36.29.72       |
| DNS Server             | 10.36.29.72       |



## Part B: Basic Networking Concepts

### What is an IP Address?

An IP Address is a unique identifier assigned to a device on a network that allows communication between devices.

### What is a MAC Address?

A MAC Address is a unique hardware address assigned to a network interface card (NIC) for identification within a local network.

### What is a Default Gateway?

A Default Gateway is a router or network device that forwards traffic from a local network to other networks, including the internet.

### What is DNS?

DNS (Domain Name System) translates domain names such as google.com into IP addresses that computers can understand.

### Public IP vs Private IP

| Public IP                    | Private IP                          |
| ---------------------------- | ----------------------------------- |
| Accessible over the internet | Used within a local network         |
| Assigned by ISP              | Assigned by router/network          |
| Globally unique              | Can be reused in different networks |


## Part C: Network Diagram

### Network Structure

Internet
↓
ISP Network
↓
Router / Gateway (10.36.29.72)
↓
Laptop - SAYALI (10.36.29.107)

A network diagram image is included in the repository .



## Part D: Network Connectivity Test

### Commands Used


ipconfig
ping google.com
tracert google.com

### Ping Test Results

* Ping was successful.
* Packets Sent: 4
* Packets Received: 4
* Packet Loss: 0%

### Traceroute Results

* Destination: google.com
* Total Hops Reached: 18
* Trace completed successfully.

### Purpose of Traceroute

Traceroute is used to identify the path taken by network packets from a source device to a destination server. It helps diagnose network delays and connectivity issues by displaying each hop along the route.

---

## Screenshot Evidence

The repository contains screenshots of:

* ipconfig /all output
* Ping test results
* Traceroute results
* Network diagram

All screenshots are available in the **Screenshots** folder.


## Conclusion

This task helped me understand the basic components of a computer network, including IP addressing, MAC addresses, DNS, gateways, and network connectivity testing. I also learned how to use command-line networking tools such as ipconfig, ping, and tracert to analyze network configuration and connectivity.

---

**Submitted as part of the White Band Associates Cyber Security Summer Internship Program.**

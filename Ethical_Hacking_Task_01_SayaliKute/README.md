# Ethical Hacking Task 01: Passive Reconnaissance

**Date:** 25 June 2026
**Name:** Sayali Kute

---

# 🎯 Task Objective

The objective of this task was to understand the reconnaissance phase of ethical hacking by collecting publicly available information about a target website using passive reconnaissance techniques. The task focused on gathering domain information, DNS records, website technologies, HTTP security headers, and publicly accessible configuration files without interacting directly with the target system.

---

# 🌐 Target Information

| Parameter           | Value                         |
| ------------------- | ----------------------------- |
| Target Website      | Government Polytechnic Nashik |
| Domain              | gpnashik.ac.in                |
| Website URL         | https://gpnashik.ac.in        |
| Reconnaissance Type | Passive Reconnaissance        |

---

# 🔍 WHOIS Summary

A WHOIS lookup was performed to collect publicly available domain registration information.

* **Registrar:** ERNET India
* **Registration Date:** 14 February 2017
* **Expiry Date:** 14 February 2029
* **Domain Status:** OK
* **Name Servers:** christian.ns.cloudflare.com, irma.ns.cloudflare.com

**Observation:**
The domain is actively registered and uses Cloudflare name servers for DNS management and website protection.

---

# 🌍 DNS Summary

DNS enumeration identified the following records:

### A Records

* 104.21.6.107
* 172.67.134.187

### MX Records

* aspmx.l.google.com
* alt1.aspmx.l.google.com
* alt2.aspmx.l.google.com
* alt3.aspmx.l.google.com
* alt4.aspmx.l.google.com

### NS Records

* christian.ns.cloudflare.com
* irma.ns.cloudflare.com

### TXT Record

* No publicly available TXT record found.

**Observation:**
Cloudflare is used for DNS hosting and security, while Google Workspace manages the domain's email services.

---

# 💻 Technology Summary

Website technology identification revealed the following:

| Technology           | Result                                   |
| -------------------- | ---------------------------------------- |
| CMS                  | No CMS Detected                          |
| Programming Language | PHP 8.3.30                               |
| CDN                  | Cloudflare                               |
| JavaScript Libraries | jsDelivr, cdnjs, Google Hosted Libraries |

**Observation:**
The website appears to be a custom-developed PHP application and uses Cloudflare and multiple CDN services to improve security and website performance.

---

# 🛡️ Security Headers Summary

The website was analyzed using **SecurityHeaders.com**.

| Header                    | Status  |
| ------------------------- | ------- |
| Content-Security-Policy   | Present |
| Strict-Transport-Security | Missing |
| X-Frame-Options           | Missing |
| X-Content-Type-Options    | Missing |
| Referrer-Policy           | Missing |
| Permissions-Policy        | Missing |

**Overall Security Grade:** **D**

**Observation:**
The website has implemented Content-Security-Policy (CSP), but several recommended HTTP security headers are missing. Implementing these headers would improve protection against common web attacks.

---

# 📄 Robots.txt Summary

The website contains a **robots.txt** file that provides instructions for search engine crawlers.

No publicly accessible **sitemap.xml** file was found during the reconnaissance process.

**Observation:**
The robots.txt file helps control search engine crawling and indexing, while the absence of a sitemap means search engines rely on internal links to discover website pages.

---

# 📚 Learning Outcome

Through this task, I learned:

* The importance of passive reconnaissance in ethical hacking.
* How to perform WHOIS lookups and analyze domain registration information.
* How DNS records provide information about website infrastructure.
* How to identify website technologies using publicly available tools.
* The role of HTTP security headers in protecting web applications.
* The purpose of robots.txt and sitemap files.
* The importance of conducting reconnaissance ethically without attempting unauthorized access.

---

# 📁 Repository Contents

* Reconnaissance Report
* Documentation Report
* WHOIS Results
* DNS Enumeration Results
* Technology Identification
* Security Headers Analysis
* Robots.txt Findings
* Screenshots
* README.md

---

# ✅ Conclusion

This task provided practical experience in the reconnaissance phase of ethical hacking using only publicly available information. I successfully gathered domain registration details, DNS records, website technologies, security header information, and robots.txt findings without performing any intrusive activities. The exercise demonstrated how valuable information about a website's infrastructure can be collected through passive techniques while respecting ethical and legal boundaries. Overall, this task strengthened my understanding of reconnaissance methodologies, information gathering tools, and the importance of responsible cybersecurity practices.

---

**Submitted as part of the White Band Associates Cyber Security Summer Internship Program.**

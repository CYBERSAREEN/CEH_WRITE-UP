# 🔐 REPORTS_DVWA-BWAPP_POC

> **Comprehensive Vulnerability Reports & Proof-of-Concept Exploits**
> Covering all DVWA and bWAPP vulnerabilities mapped to CVE · CWE · CVSS

![Status](https://img.shields.io/badge/Status-Active-brightgreen)
![Platform](https://img.shields.io/badge/Platform-DVWA%20%7C%20bWAPP-blue)
![License](https://img.shields.io/badge/License-MIT-lightgrey)
![Author](https://img.shields.io/badge/Author-Vedant%20Sareen-purple)

---

## 📌 About This Repository

This repository is a structured collection of **professional-grade penetration testing reports and Proof-of-Concept (PoC) exploits** for every vulnerability present in:

- **DVWA** (Damn Vulnerable Web Application)
- **bWAPP** (Buggy Web Application)

Each entry is formally documented with its corresponding **CVE**, **CWE**, and **CVSS v3.1 score**, following industry-standard reporting practices used in real-world penetration testing engagements.

> This repository is intended purely for **educational purposes**, **security research**, and **ethical hacking practice** in controlled, authorized environments.

---

## 🗂️ Repository Structure

```
REPORTS_DVWA-BWAPP_POC/
│
├── DVWA/
│   ├── SQL_Injection/
│   │   ├── report.md
│   │   ├── poc.md
│   │   └── screenshots/
│   ├── XSS_Reflected/
│   ├── XSS_Stored/
│   ├── XSS_DOM/
│   ├── CSRF/
│   ├── File_Upload/
│   ├── File_Inclusion/
│   ├── Command_Injection/
│   ├── Brute_Force/
│   ├── IDOR/
│   └── Weak_Session_IDs/
│
├── bWAPP/
│   ├── HTML_Injection/
│   ├── SQL_Injection/
│   ├── XXE_Injection/
│   ├── SSRF/
│   ├── Open_Redirect/
│   ├── LDAP_Injection/
│   ├── OS_Command_Injection/
│   ├── PHP_Injection/
│   ├── Server_Side_Template_Injection/
│   ├── XML_Injection/
│   ├── iFrame_Injection/
│   ├── Clickjacking/
│   ├── CORS_Misconfiguration/
│   └── Insecure_DOR/
│
├── templates/
│   ├── report_template.md
│   └── poc_template.md
│
└── README.md
```

---

## 📊 Vulnerability Coverage Index

### 🔴 DVWA

| #  | Vulnerability                  | CWE     | CVE (Reference) | CVSS v3.1 | Severity | Report | PoC |
| -- | ------------------------------ | ------- | --------------- | --------- | -------- | ------ | --- |
| 1  | SQL Injection                  | CWE-89  | CVE-2012-1823   | 9.8       | Critical | ⬜     | ⬜  |
| 2  | Blind SQL Injection            | CWE-89  | CVE-2012-1823   | 9.8       | Critical | ⬜     | ⬜  |
| 3  | XSS (Reflected)                | CWE-79  | CVE-2023-32315  | 6.1       | Medium   | ⬜     | ⬜  |
| 4  | XSS (Stored)                   | CWE-79  | CVE-2023-32315  | 8.0       | High     | ⬜     | ⬜  |
| 5  | XSS (DOM)                      | CWE-79  | CVE-2023-32315  | 6.1       | Medium   | ⬜     | ⬜  |
| 6  | CSRF                           | CWE-352 | CVE-2020-11022  | 6.5       | Medium   | ⬜     | ⬜  |
| 7  | File Upload                    | CWE-434 | CVE-2021-44228  | 9.8       | Critical | ⬜     | ⬜  |
| 8  | File Inclusion (LFI/RFI)       | CWE-98  | CVE-2012-1823   | 9.8       | Critical | ⬜     | ⬜  |
| 9  | Command Injection              | CWE-78  | CVE-2014-6271   | 10.0      | Critical | ⬜     | ⬜  |
| 10 | Brute Force                    | CWE-307 | CVE-2019-11043  | 7.5       | High     | ⬜     | ⬜  |
| 11 | IDOR                           | CWE-639 | CVE-2020-24553  | 5.4       | Medium   | ⬜     | ⬜  |
| 12 | Weak Session IDs               | CWE-330 | CVE-2020-7699   | 7.5       | High     | ⬜     | ⬜  |
| 13 | JavaScript Attacks             | CWE-345 | —              | 5.3       | Medium   | ⬜     | ⬜  |
| 14 | Content Security Policy Bypass | CWE-693 | —              | 6.1       | Medium   | ⬜     | ⬜  |

### 🟠 bWAPP

| #  | Vulnerability                    | CWE      | CVE (Reference) | CVSS v3.1 | Severity | Report | PoC |
| -- | -------------------------------- | -------- | --------------- | --------- | -------- | ------ | --- |
| 1  | HTML Injection (Reflected)       | CWE-80   | —              | 6.1       | Medium   | ⬜     | ⬜  |
| 2  | HTML Injection (Stored)          | CWE-80   | —              | 8.0       | High     | ⬜     | ⬜  |
| 3  | SQL Injection (GET/POST)         | CWE-89   | CVE-2012-1823   | 9.8       | Critical | ⬜     | ⬜  |
| 4  | SQL Injection (AJAX/JSON)        | CWE-89   | CVE-2012-1823   | 9.8       | Critical | ⬜     | ⬜  |
| 5  | XXE Injection                    | CWE-611  | CVE-2021-44228  | 9.1       | Critical | ⬜     | ⬜  |
| 6  | SSRF                             | CWE-918  | CVE-2021-26855  | 9.8       | Critical | ⬜     | ⬜  |
| 7  | LDAP Injection                   | CWE-90   | —              | 7.5       | High     | ⬜     | ⬜  |
| 8  | OS Command Injection             | CWE-78   | CVE-2014-6271   | 10.0      | Critical | ⬜     | ⬜  |
| 9  | PHP Code Injection               | CWE-94   | —              | 9.8       | Critical | ⬜     | ⬜  |
| 10 | Server-Side Template Injection   | CWE-94   | CVE-2022-22954  | 9.8       | Critical | ⬜     | ⬜  |
| 11 | XML Injection                    | CWE-91   | —              | 7.5       | High     | ⬜     | ⬜  |
| 12 | iFrame Injection                 | CWE-79   | —              | 6.1       | Medium   | ⬜     | ⬜  |
| 13 | Open Redirect                    | CWE-601  | CVE-2022-33891  | 6.1       | Medium   | ⬜     | ⬜  |
| 14 | Clickjacking                     | CWE-1021 | —              | 4.3       | Medium   | ⬜     | ⬜  |
| 15 | CORS Misconfiguration            | CWE-942  | —              | 7.4       | High     | ⬜     | ⬜  |
| 16 | Insecure Direct Object Reference | CWE-639  | —              | 5.4       | Medium   | ⬜     | ⬜  |
| 17 | Unrestricted File Upload         | CWE-434  | —              | 9.8       | Critical | ⬜     | ⬜  |
| 18 | Sensitive Data Exposure          | CWE-200  | —              | 7.5       | High     | ⬜     | ⬜  |
| 19 | Broken Auth / Session Mgmt       | CWE-287  | —              | 9.8       | Critical | ⬜     | ⬜  |
| 20 | Security Misconfiguration        | CWE-16   | —              | 7.5       | High     | ⬜     | ⬜  |

> ✅ = Completed &nbsp;&nbsp; 🔄 = In Progress &nbsp;&nbsp; ⬜ = Pending

---

## 📄 Report Format (Per Vulnerability)

Each report follows this structure:

```
## Vulnerability Name
- Target Application: DVWA / bWAPP
- Severity: Critical / High / Medium / Low
- CWE: CWE-XXX (Category Name)
- CVSS v3.1 Score: X.X
- CVSS Vector: AV:N/AC:L/PR:N/UI:N/S:U/C:H/I:H/A:H

### Description
### Steps to Reproduce
### Payload Used
### Screenshots / Evidence
### Impact Analysis
### Remediation
### References
```

---

## 🧪 Testing Environment

| Component        | Details                     |
| ---------------- | --------------------------- |
| OS               | Kali Linux 2024.x           |
| DVWA Version     | 1.10 / Latest               |
| bWAPP Version    | 2.2                         |
| Deployment       | Docker / XAMPP / VirtualBox |
| Browser          | Firefox (with FoxyProxy)    |
| Proxy            | Burp Suite Community / Pro  |
| Additional Tools | SQLMap, Nikto, FFUF, Nmap   |

---

## ⚙️ Setup & Usage

```bash
# Clone this repository
git clone https://github.com/YourUsername/REPORTS_DVWA-BWAPP_POC.git
cd REPORTS_DVWA-BWAPP_POC

# Run DVWA with Docker
docker run --rm -it -p 80:80 vulnerables/web-dvwa

# Run bWAPP with Docker
docker run -d --name bwapp -p 8080:80 raesene/bwapp
# Default credentials: bee / bug
```

---

## 🛡️ Disclaimer

> ⚠️ **This repository is strictly for educational and authorized security research purposes.**
> All vulnerabilities documented here were tested in **isolated, local lab environments**.
> **Do NOT** use these techniques against any system without **explicit written authorization**.
> The author holds no responsibility for any misuse of this content.

---

## 👤 Author

**Vedant Sareen**
B.Tech CSE (Cybersecurity) — Chitkara University, Punjab
📧 securecybernetics@gmail.com
🔗 [LinkedIn](https://linkedin.com/in/yourprofile) · [GitHub](https://github.com/YourUsername)

---

## 📜 License

This project is licensed under the [MIT License](LICENSE).

---

<p align="center">
  <i>"Security is not a product, but a process." — Bruce Schneier</i>
</p>

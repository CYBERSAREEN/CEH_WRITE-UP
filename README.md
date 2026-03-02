# 🛡️ CEH Practical Lab Writeups & Tools
### Complete Hands-On Walkthrough — All 20 Modules | EC-Council CEH v13

> **Author:** Vedant Sareen (CYBERSAREEN)
> **Institution:** Chitkara University, Punjab, India
> **Contact:** securecybernetics@gmail.com
> **GitHub:** [github.com/CYBERSAREEN](https://github.com/CYBERSAREEN)

![Status](https://img.shields.io/badge/Status-Active%20Daily%20Writeups-brightgreen)
![Labs](https://img.shields.io/badge/Labs%20Covered-1%2F20-blue)
![Platform](https://img.shields.io/badge/Platform-Kali%20%7C%20ParrotOS%20%7C%20Windows-red)
![License](https://img.shields.io/badge/License-MIT-lightgrey)

---

> ⚠️ **Disclaimer:** All content in this repository is strictly for **educational purposes** and **authorized security research** only. All labs are performed in isolated, controlled lab environments. The author is not responsible for any misuse of this material by readers.

---

## 📌 About This Repository

This repository is a **daily-updated, practical CEH lab journal** — every module is documented as a professional-grade writeup covering the scenario, methodology, tools used, commands executed, observations, and key takeaways.

Where a lab demands a custom tool or script, a working implementation is pushed alongside the writeup.

The goal is simple: **turn every lab into a reference-grade document** that bridges the gap between theory and real-world ethical hacking practice.

---

## 🗂️ Repository Structure

```
CEH-Lab-Writeups/
│
├── Module_01_Footprinting_Reconnaissance/
│   ├── Lab-01_Google_Hacking/
│   │   ├── writeup.md
│   │   └── screenshots/
│   ├── Lab-02_Netcraft_DNSdumpster/
│   ├── Lab-03_Sherlock_Whois/
│   ├── Lab-04_DomainTools_WHOIS/
│   ├── Lab-05_nslookup_DNS/
│   ├── Lab-06_Traceroute/
│   ├── Lab-07_eMailTrackerPro/
│   ├── Lab-08_Recon-ng/
│   └── Lab-09_ShellGPT/
│
├── Module_02_Scanning_Networks/
├── Module_03_Enumeration/
├── Module_04_Vulnerability_Analysis/
├── Module_05_System_Hacking/
├── Module_06_Malware_Threats/
├── Module_07_Sniffing/
├── Module_08_Social_Engineering/
├── Module_09_DoS_DDoS/
├── Module_10_Session_Hijacking/
├── Module_11_Evading_IDS_Firewalls/
├── Module_12_Hacking_Web_Servers/
├── Module_13_Hacking_Web_Apps/
├── Module_14_SQL_Injection/
├── Module_15_Hacking_Wireless/
├── Module_16_Hacking_Mobile/
├── Module_17_IoT_OT_Hacking/
├── Module_18_Cloud_Computing/
├── Module_19_Cryptography/
├── Module_20_AI_in_Cybersecurity/
│
├── tools/                        ← Custom scripts pushed per lab demand
│   └── README.md
│
└── README.md
```

---

## 📊 Module Progress Tracker

| # | Module | Labs | Status | Last Updated |
|---|--------|------|--------|-------------|
| 01 | 🔍 Footprinting & Reconnaissance | 9 | ✅ Complete | 02-03-2026 |
| 02 | 🌐 Scanning Networks | — | ⬜ Pending | — |
| 03 | 📋 Enumeration | — | ⬜ Pending | — |
| 04 | 🔬 Vulnerability Analysis | — | ⬜ Pending | — |
| 05 | 💻 System Hacking | — | ⬜ Pending | — |
| 06 | 🦠 Malware Threats | — | ⬜ Pending | — |
| 07 | 👃 Sniffing | — | ⬜ Pending | — |
| 08 | 🎭 Social Engineering | — | ⬜ Pending | — |
| 09 | 💥 DoS / DDoS | — | ⬜ Pending | — |
| 10 | 🔗 Session Hijacking | — | ⬜ Pending | — |
| 11 | 🚧 Evading IDS, Firewalls & Honeypots | — | ⬜ Pending | — |
| 12 | 🌍 Hacking Web Servers | — | ⬜ Pending | — |
| 13 | 🕸️ Hacking Web Applications | — | ⬜ Pending | — |
| 14 | 💉 SQL Injection | — | ⬜ Pending | — |
| 15 | 📶 Hacking Wireless Networks | — | ⬜ Pending | — |
| 16 | 📱 Hacking Mobile Platforms | — | ⬜ Pending | — |
| 17 | 🔌 IoT & OT Hacking | — | ⬜ Pending | — |
| 18 | ☁️ Cloud Computing | — | ⬜ Pending | — |
| 19 | 🔐 Cryptography | — | ⬜ Pending | — |
| 20 | 🤖 AI in Cybersecurity | — | ⬜ Pending | — |

> ✅ Complete &nbsp;|&nbsp; 🔄 In Progress &nbsp;|&nbsp; ⬜ Pending

---

## ✅ Module 01 — Footprinting & Reconnaissance

> *"Know your target before they know you're watching."*

| Lab | Topic | Tools Used | Writeup | Custom Tool |
|-----|-------|-----------|---------|-------------|
| 1-01 | Advanced Google Hacking Techniques | Google Dorks, GHDB | ✅ | — |
| 1-02 | Domain, Subdomain & Host Discovery | Netcraft, DNSdumpster | ✅ | — |
| 1-03 | Social Media OSINT & Domain Recon | Sherlock, Whois | ✅ | — |
| 1-04 | WHOIS Lookup & Domain Authenticity | DomainTools | ✅ | — |
| 1-05 | DNS Enumeration via nslookup | nslookup, kloth.net | ✅ | — |
| 1-06 | Network Tracerouting | tracert, traceroute, SolarWinds | ✅ | — |
| 1-07 | Email Tracing & Header Analysis | eMailTrackerPro | ✅ | — |
| 1-08 | Automated Footprinting | Recon-ng | ✅ | — |
| 1-09 | AI-Assisted OSINT | ShellGPT | ✅ | — |

### Key Google Dorks Reference (Lab 1-01)

```bash
# Login portal enumeration
intitle:login site:target.com
inurl:login site:target.com

# Employee & contact discovery
allinurl: target-company employee_name
inanchor:contact site:target.com

# LinkedIn references
link:linkedin site:target.com

# Files containing sensitive info (from GHDB)
intext:"user" filetype:php intext:"account" inurl:/admin
intitle:"index of" "username.txt"
filetype:reg reg HKEY_CURRENT_USER SSHHOSTKEYS
```

### DNS Record Quick Reference (Lab 1-05)

```bash
nslookup
> set type=A        # IPv4 address
> set type=MX       # Mail servers
> set type=NS       # Name servers
> set type=TXT      # SPF/DKIM records
> set type=AXFR     # Zone transfer attempt (CRITICAL)
> target.com
```

### Recon-ng Quick Workflow (Lab 1-08)

```bash
recon-ng
> workspaces create target
> db insert domains → target.com
> marketplace install recon/domains-hosts/hackertarget
> modules load recon/domains-hosts/hackertarget
> options set SOURCE target.com
> run
> show hosts
```

---

## 🧰 Tools Index

Custom scripts and tools pushed alongside labs when required:

| Tool | Lab | Description | Language |
|------|-----|-------------|----------|
| *(Coming soon)* | — | — | — |

> Tools are added on demand as labs require custom automation or scripting beyond standard platform tools.

---

## 🖥️ Lab Environment

| Component | Details |
|-----------|---------|
| Primary Attack OS | Kali Linux 2024.x / ParrotOS |
| Target Environments | Metasploitable 2/3, DVWA, bWAPP, Windows Server 2019 AD |
| Virtualization | VirtualBox / VMware Workstation |
| Network | NAT + Host-Only isolated lab network |
| Browser | Firefox + FoxyProxy |
| Proxy | Burp Suite Community / Pro |
| AI Assistant | ShellGPT (OpenAI API) |

---

## 📝 Writeup Format

Every lab writeup follows this structure for consistency and professional quality:

```
## Lab X-XX: [Lab Title]

### Scenario
### Objective
### Tools Used
### Phase 1: [Phase Name]
  - Methodology
  - Commands / Queries
  - Screenshots
### Phase 2: [Phase Name]
### Key Findings
### Risk Assessment
### Mitigation Recommendations
### Personal Notes & Observations
```

---

## 🔗 Related Repositories

| Repository | Description |
|------------|-------------|
| [REPORTS_DVWA-BWAPP_POC](https://github.com/CYBERSAREEN/REPORTS_DVWA-BWAPP_POC) | Vulnerability reports & PoCs for DVWA and bWAPP mapped to CVE/CWE/CVSS |

---

## 👤 Author

**Vedant Sareen**
B.Tech CSE (Cybersecurity) — Chitkara University, Punjab, India
📧 securecybernetics@gmail.com
🔗 [GitHub](https://github.com/CYBERSAREEN)

---

## 📜 License

This repository is licensed under the [MIT License](LICENSE).
All writeups and tools are for educational and authorized security research purposes only.

---

<p align="center">
  <i>"The quieter you become, the more you can hear."</i><br>
  <b>— Kali Linux Motto</b>
</p>

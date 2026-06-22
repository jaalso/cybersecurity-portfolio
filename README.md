
# 👾Cybersecurity Portfolio

> Aim of this repo is to display the different projects I've worked on during the last months.

## About Me
A cybersecurity learner enrolled in the CSS EFA Program at SCI, building hands-on skills across both offensive (red team) and defensive (blue team) disciplines. 
My background is in IT Infrastructure, System Admin, Network, Automation, IT Support and I'm currently focused on transitioning into a SOC Analyst or Penetration Tester role in Switzerland.

- 🎯 Currently studying: Ethical Hacking, SIEM, Malware Analysis, Phishing Simulation
- 🚩Swiss Cyber Institute modules completed: Communication & Leadership, ATT&CK Frameworks, Risk Rating (CIA/CVSS/CVE/DREAD), Vulnerability Scanning, Network Analysis, Scan & Simulate Attacks, Certification & Encryption, Network Basic & Analysis, Basic Hardening, Email Communication Investigation, Intrusion Detection Systems, IR Playbooks, Triage, Web App Security and Web Hardening, Python. 
- 🛡️ Platforms: TryHackMe · HackTheBox · PortSwigger · JuiceShop · CyberDefenders · LetsDefend 
- 🔬 My Own Security Labs: GNS3, WMware Workstation Pro, VirtualBox, Vulnerable VMs.  
- 📬 Open to: security engineering, ethical hacking, junior penetration testing. I work across both sides — building detections and doing host forensics on the blue team, and enumeration-to-exploitation labs on the red team — because understanding one makes you better at the other.

---

## 🔴 [Red Team Labs](https://github.com/jaalso/red-team-labs) <sup><sub>← click to open</sub></sup>
> Offensive security · Penetration testing · Exploitation · Phishing simulation

| # | Lab | Tools | Status |
|---|---|---|---|
| 01 | Network Penetration Testing | nmap · Metasploit · Hydra | ✅ Complete |
| 02 | GoPhish Phishing Simulation & Offensive Email Attack Chain | GoPhish · Zphisher · SET · Ngrok · Cloudflared · Postfix | ✅ Complete  |
| 03 | WordPress Full Compromise (Bigware/Dockerlabs) — CVE-2025-34077 | nmap · WPScan · Metasploit · netcat | ✅ Complete |
| 04 | WordPress Purple Team — CVE-2020-25213 | curl · bash · Apache logs · mimipenguin | ✅ Complete |
| 05 | Web App Security Analysis (Burp Suite / OWASP ZAP)	Burp Suite · OWASP ZAP  |  Browser DevTools | 	🔜 Coming soon | 
---

## 🛡️ [Blue Team Labs](https://github.com/jaalso/blue-team-labs) <sup><sub>← click to open</sub></sup>
> Forensics · SIEM · Network analysis · Certificate auditing · Email security

| # | Lab | Tools | Status |
|---|---|---|---|
| 01 | Network Traffic Forensics (Phishing PCAP) | Wireshark · TShark · VirusTotal | ✅ Complete |
| 02 | Home Network Security Audit | netdiscover · nmap · Hydra | ✅ Complete |
| 03 | Web App Security — Certificate Analysis | nmap NSE · sslyze · openssl | ✅ Complete |
| 04 | SIEM & Endpoint Detection (Wazuh) | Wazuh v4.14.3 · OpenSearch (internal) · systemctl · SSH | ✅ Complete |
| 05 | Email Security Gateway — Proxmox Mail Gateway | Docker · Postfix · PMG · swaks · Thunderbird | ✅ Complete |
| 06 | Automated Windows Triage Tool — Invoke-CompromiseCheck.ps1 | PowerShell · CIM/WMI · Event Log · auditpol | ✅ Complete |

---

## 🔍 [Incident Response Labs](https://github.com/jaalso/incident-response-labs) <sup><sub>← click to open</sub></sup>
> DFIR · Windows forensics · Attack simulation · IR reporting

| # | Lab | Tools | Status |
|---|---|---|---|
| 01 | SMB Brute Force Attack & Windows Forensics | CrackMapExec · EZ Tools · EvtxECmd | ✅ Complete |
| 02 | Wayne Corp IR Simulation — Windows DFIR & SOC | KAPE · EZ Tools · impacket · Timeline Explorer | ✅ Complete |

---

## 🌐 [Web Security Labs](https://github.com/jaalso/web-security) <sup><sub>← click to open</sub></sup>

> SQL injection · XSS · CSP · Apache hardening · OWASP Juice Shop · PortSwigger Web Security Academy

| # | Lab | Tools | Status |
|---|---|---|---|
| 01 | SQL Injection — Auth Bypass & UNION Extraction | Burp Suite · Juice Shop · PortSwigger | ✅ Complete |
| 02 | Broken Access Control — IDOR, Path Traversal & Forged Review | Burp Suite · Intruder · PortSwigger | ✅ Complete |
| 03 | XSS & Content Security Policy Defence | DevTools · Juice Shop · PortSwigger | ✅ Complete |
| 04 | Apache Web Server Hardening | Apache · mod_headers · Nikto · curl | ✅ Complete |

---

## 🔬 [Security Research](https://github.com/jaalso/security-research) <sup><sub>← click to open</sub></sup>
> Independent threat verification · Privacy analysis · Regulatory context

| # | Research | Type | Status |
|---|---|---|---|
| 01 | BrowserGate — LinkedIn Browser Fingerprinting | Threat Verification + Privacy | ✅ Complete |
| 02 | Booking.com Storm-1865 Phishing Triage | Live CTI · Incident Prevention · NCSC Report | ✅ Complete |
| 03 | Windows Telemetry — What Microsoft Sees from a Personal Host | PowerShell · Privacy Dashboard · GDPR Analysis | ✅ Complete |

---

## 🐍 [Security Scripts](https://github.com/jaalso/security-scripts) <sup><sub>← click to open</sub></sup>

> Python automation for offensive and defensive security operations · Swiss Cyber Institute Module 7

| # | Tool | Description | Status |
|---|---|---|---|
| 01 | log-enricher | IP geolocation enrichment · non-Swiss access flagging | ✅ Complete |
| 02 | hashfile.py | SHA-256 · SHA-1 · MD5 hash computation for file triage | 🔜 Planned |
| 03 | dnslookup.py | Bulk DNS A-record resolution with suspicious TLD detection | 🔜 Planned |
| 04 | certinfo.py | TLS certificate subject · issuer · expiry extraction | 🔜 Planned |
| 05 | urlrep.py | URL reputation via URLscan.io + VirusTotal API | 🔜 Planned |

---

## 🧠 [Memory Forensics Labs](https://github.com/jaalso/memory-forensics-labs) <sup><sub>← click to open</sub></sup>
> Windows memory forensics · Volatility 2 · Malware analysis · DFIR

| # | Case | Malware | Technique | Status |
|---|---|---|---|---|
| 01 | Cridex Banking Trojan | Cridex / Bugat | Process injection · C2 detection | ✅ Complete |
| 02 | Zeus / Zbot Banking Trojan | Zeus / Zbot | malfind · vaddump · persistence | ✅ Complete |

---

## 🧰 Tools & Technologies

| Category | Tools |
|---|---|
| Scanning & Recon | nmap · netdiscover · Wireshark · TShark · NetworkMiner · Wappalyzer |
| Exploitation | Metasploit · Hydra · CrackMapExec |
| Web App Testing | WPScan · Burp Suite · OWASP ZAP · curl · searchsploit · Nikto |
| Web Security | OWASP Juice Shop · PortSwigger Web Security Academy · FoxyProxy · ModHeader |
| CVE Exploitation | Python3 PoC · CVE-2025-34077 · CVE-2020-25213 |
| Certificate Analysis | nmap NSE · sslyze · sslscan · openssl · telnet · csvlook |
| SIEM & Monitoring | Wazuh v4.14.3 · OpenSearch (internal) |
| Email Forensics | emlAnalyzer · CyberChef · MXToolbox · analyze.py |
| Phishing Simulation | GoPhish · Zphisher · SET · swaks |
| Email Gateway | Proxmox Mail Gateway · Postfix · Dovecot · SpamAssassin · ClamAV |
| Tunneling | Ngrok · Cloudflared · LocalXpose |
| Windows Forensics | PECmd · AmcacheParser · AppCompatCacheParser · EvtxECmd |
| Post-Exploitation | Metasploit shell · netcat · mimipenguin |
| Privacy Research | Chrome DevTools · Brave Browser · EFF CoverYourTracks |
| Containerization | Docker · docker-compose |
| Scripting | Python 3.13 · PowerShell · Bash · requests · csv |
| Platforms | Kali Linux · Windows 10/11 · Metasploitable 2 · VirtualBox · Docker |

---

# Certifications & Training
- 🎓 Swiss Cyber Institute — Cybersecurity Specialist Program (in progress)
- 🎓 Swiss Cyber Institute — Certified Security Professional Training (completed) 
 


## 🌐 Find Me On
[![TryHackMe](https://img.shields.io/badge/TryHackMe-jaalsove-red?style=for-the-badge&logo=tryhackme)](https://tryhackme.com/p/jaalsove)
[![HackTheBox](https://img.shields.io/badge/HackTheBox-Bornia01-9FEF00?style=for-the-badge&logo=hackthebox&logoColor=black)](https://profile.hackthebox.com/profile/019c9973-b580-718e-adda-fcdc2795deb3)
[![PortSwigger](https://img.shields.io/badge/PortSwigger-Web%20Security%20Academy-orange?style=for-the-badge)](https://github.com/jaalso/web-security#01--sql-injection--auth-bypass--union-extraction)
[![JuiceShop](https://img.shields.io/badge/OWASP-Juice%20Shop-brightgreen?style=for-the-badge)](https://github.com/jaalso/web-security#03--xss--content-security-policy-defence)
[![CyberDefenders](https://img.shields.io/badge/CyberDefenders-bornia01-blue?style=for-the-badge)](https://cyberdefenders.org/p/bornia01/)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Jaime%20Soto-0077B5?style=for-the-badge&logo=linkedin)](https://linkedin.com/in/jaalso)

## ⚖️Legal & Ethical Notice
All penetration testing and offensive security activities documented in this portfolio were conducted exclusively in:

- Isolated personal lab environments (VMs with no external connectivity)
- Authorized external targets (vuln.land)
- Simulated environments provided by training platforms (THM, HTB)

No unauthorized systems were accessed. All work complies with Swiss law and ethical hacking standards.

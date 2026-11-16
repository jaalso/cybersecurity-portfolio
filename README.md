# 👾 About me
Breaking into offensive & defensive security from a system admin / IT infrastructure (banking & enterprise) background. This is where I publish lab write-ups, CTF solutions, and notes, the honest version, with tutorials credited where followed.

<br>**📬 Open** to: SOC analyst / blue team / detection, endpoint investigation / incident response.
<br>**Links:** [Lab portfolio](https://jaalso.github.io/labs/) · [LinkedIn](https://linkedin.com/in/jaalso) · [HackTheBox](https://profile.hackthebox.com/profile/019c9973-b580-718e-adda-fcdc2795deb3) · [TryHackMe](https://tryhackme.com/p/jaalsove) · [CyberDefenders](https://cyberdefenders.org/p/bornia01/)

---

**CEH** · In Progress
<br>**CSS EFA Bachelor** · SCI 
<br>**Google Cyber Security** 
<br>**CSP** · SCI 
<br>**NCSC Switzerland** · acknowledged real-world CTI investigation (Storm-1865, May 2026)

---

## Blue-team work to start with

| Area | What I did | Where |
|---|---|---|
| SIEM and endpoint monitoring | Deployed and operated Wazuh v4.14.3 with OpenSearch; CIS Benchmark review (190 controls) | [Blue Team Labs](https://github.com/jaalso/blue-team-labs) |
| Host triage and DFIR | KAPE collection (3,303 artifacts in 13 minutes), Eric Zimmerman tools, full attack-chain reconstruction after SMB brute force and PsExec lateral movement | [Incident Response Labs](https://github.com/jaalso/incident-response-labs) |
| Windows triage automation | PowerShell tool (`Invoke-CompromiseCheck.ps1`) using CIM/WMI, event logs and audit policy | [Blue Team Labs](https://github.com/jaalso/blue-team-labs) |
| Network and email analysis | Phishing PCAP forensics, email header and MIME analysis, Proxmox Mail Gateway | [Blue Team Labs](https://github.com/jaalso/blue-team-labs) |
| Memory forensics | Volatility 2 and 3 on Cridex and Zeus/Zbot images: process injection, C2 detection, persistence | [Memory Forensics](https://github.com/jaalso/memory-forensics) |
| Threat intelligence | Independent Storm-1865 phishing investigation, acknowledged by NCSC Switzerland | [Security Research](https://github.com/jaalso/security-research) |
| SOC tooling in Python | Log enrichment, SBOM scanning against OSV.dev, DNS typosquatting detection, triage helpers | [Security Scripts](https://github.com/jaalso/security-scripts) |

## Supporting areas

| Area | Evidence |
|---|---|
| Web security and hardening (OWASP Top 10, CSP, TLS, Apache) | [Web Security Labs](https://github.com/jaalso/web-security) |
| Identity and access (Keycloak, OIDC, JWT) | [IAM Labs](https://github.com/jaalso/iam-labs) |
| Offensive security (network pentest, phishing simulation, CVE-2025-34077, CVE-2020-25213) | [Red Team Labs](https://github.com/jaalso/red-team-labs) |

---

## How to read this portfolio

This is coursework, personal labs, training-platform exercises and independent investigations. It is not a history of commercial penetration-testing engagements. Each write-up states its context, my contribution, tools, evidence, findings, limitations and recommendations, and credits tutorials and external sources where I followed them.

---

## Blue Team Labs: [repo](https://github.com/jaalso/blue-team-labs)
*SIEM · network analysis · certificate auditing · email security · triage*

| # | Lab | Tools |
|---|---|---|
| 01 | Network traffic forensics (phishing PCAP) | Wireshark · TShark · VirusTotal |
| 02 | Home network security audit | netdiscover · nmap · Hydra |
| 03 | Web app security: certificate analysis | nmap NSE · sslyze · openssl |
| 04 | SIEM and endpoint detection | Wazuh v4.14.3 · OpenSearch · SSH |
| 05 | Email security gateway | Proxmox Mail Gateway · Postfix · Docker · swaks |
| 06 | Automated Windows triage tool | PowerShell · CIM/WMI · Event Log · auditpol |

## Incident Response Labs: [repo](https://github.com/jaalso/incident-response-labs)
*DFIR · Windows forensics · attack simulation · reporting*

| # | Lab | Tools |
|---|---|---|
| 01 | SMB brute force attack and Windows forensics | CrackMapExec · EZ Tools · EvtxECmd |
| 02 | Windows DFIR engagement: lateral movement and IR simulation | KAPE · EZ Tools · impacket · Timeline Explorer |

## Memory Forensics: [repo](https://github.com/jaalso/memory-forensics)

| # | Case | Technique |
|---|---|---|
| 01 | Cridex / Bugat banking trojan | Process injection · C2 detection |
| 02 | Zeus / Zbot banking trojan | malfind · vaddump · persistence |

## Security Research: [repo](https://github.com/jaalso/security-research)
*Independent threat verification · privacy analysis · regulatory context*

| # | Research | Type |
|---|---|---|
| 01 | BrowserGate: LinkedIn browser fingerprinting | Threat verification, privacy |
| 02 | Booking.com Storm-1865 phishing triage | Live CTI, incident prevention, NCSC report |
| 03 | Windows telemetry: what Microsoft sees from a personal host | PowerShell · Privacy Dashboard · GDPR analysis |

## Security Scripts: [repo](https://github.com/jaalso/security-scripts)
*Python automation for security operations (Swiss Cyber Institute Module 7)*

| # | Tool | Description |
|---|---|---|
| 01 | [log-enricher](https://github.com/jaalso/security-scripts#01--log-enricher) | Enrich CSV auth logs with IP geolocation, flag non-Swiss access |
| 02 | [sbom-scanner](https://github.com/jaalso/security-scripts#02--sbom-scanner) | Scan SBOM JSON against OSV.dev, CI/CD-friendly exit codes |
| 03 | [dns-typosquatting](https://github.com/jaalso/security-scripts#03--dns-typosquatting) | Detect typosquatted domains in DNS logs via Levenshtein distance |
| 04 | [soc-triage-helpers](https://github.com/jaalso/security-scripts#04--soc-triage-helpers) | Terminal utilities for IR: file hashing, DNS resolution |
| 05 | [xor-decrypt](https://github.com/jaalso/security-scripts#05--xor-decrypt) | Decrypt repeating-key XOR ciphertext |
| 06 | certinfo.py | TLS certificate subject, issuer, expiry (planned) |
| 07 | urlrep.py | URL reputation via URLscan.io and VirusTotal (planned) |

## Web Security Labs: [repo](https://github.com/jaalso/web-security)

| # | Lab | Tools |
|---|---|---|
| 01 | SQL injection: auth bypass and UNION extraction | Burp Suite · Juice Shop · PortSwigger |
| 02 | Broken access control: IDOR, path traversal, forged review | Burp Suite · Intruder · PortSwigger |
| 03 | XSS and Content Security Policy defence | DevTools · Juice Shop · PortSwigger |
| 04 | Apache web server hardening | Apache · mod_headers · Nikto · curl |

## IAM Labs: [repo](https://github.com/jaalso/iam-labs)

| # | Lab | Tools |
|---|---|---|
| 01 | Keycloak identity broker: OIDC Authorization Code flow | Keycloak · Docker · curl · JWT |

## Red Team Labs: [repo](https://github.com/jaalso/red-team-labs)
*Understanding the attacker side to build better detections*

| # | Lab | Tools |
|---|---|---|
| 01 | Network penetration testing | nmap · Metasploit · Hydra |
| 02 | GoPhish phishing simulation and offensive email attack chain | GoPhish · Zphisher · SET · Ngrok · Cloudflared · Postfix |
| 03 | WordPress full compromise (Bigware/Dockerlabs), CVE-2025-34077 | nmap · WPScan · Metasploit · netcat |
| 04 | WordPress purple team, CVE-2020-25213 | curl · bash · Apache logs · mimipenguin |
| 05 | Web app security analysis | See [Web Security Labs](https://github.com/jaalso/web-security) |

---

## Tools

| Category | Tools |
|---|---|
| SIEM and monitoring | Wazuh · OpenSearch |
| DFIR and forensics | KAPE · Eric Zimmerman tools (PECmd, AmcacheParser, AppCompatCacheParser, EvtxECmd, Timeline Explorer) · Volatility 2 / 3 |
| Network analysis | Wireshark · TShark · NetworkMiner · nmap · netdiscover |
| Email and phishing analysis | emlAnalyzer · CyberChef · MXToolbox · Proxmox Mail Gateway · SpamAssassin · ClamAV |
| Web and TLS | Burp Suite · OWASP ZAP · Nikto · sslyze · sslscan · openssl |
| Offensive (lab use) | Metasploit · Hydra · CrackMapExec · WPScan · GoPhish · SET |
| Scripting | Python 3 · PowerShell · Bash |
| Platforms | Kali Linux · Windows 10/11 · VirtualBox · Docker |

---

## Legal and ethical notice

All offensive security activity documented here was conducted only in:

- isolated personal lab environments (VMs with no external connectivity)
- authorised external targets (vuln.land, Dockerlabs)
- simulated environments provided by training platforms (THM, HTB)

No unauthorised systems were accessed. All work complies with Swiss law and ethical hacking standards.

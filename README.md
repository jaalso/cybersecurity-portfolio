
# 👾Cybersecurity Portfolio

> Aim of this repo is to display the different projects I've worked on during the last months.

## 🧭 About Me
A cybersecurity learner enrolled in the CSS EFA Program at SCI, building hands-on skills across both offensive (red team) and defensive (blue team) disciplines. 
My background is in IT infrastructure, System Admin, Network, Automation, IT Support and I'm currently focused on transitioning into a SOC Analyst or Penetration Tester role in Switzerland.

- 🎯 Currently studying: Ethical Hacking, SIEM, Malware Analysis, Phishing Simulation
- Swiss Cyber Institute modules completed: Communication & Leadership, ATT&CK Frameworks, Risk Rating (CIA/CVSS/CVE/DREAD), Vulnerability Scanning, Network Analysis, Scan & Simulate Attacks, Certification & Encryption, Network Basic & Analysis, Basic Hardening, Email Communication Investigation, Intrusion Detection Systems.
- 🛡️ Platforms: TryHackMe · HackTheBox · CyberDefenders · LetsDefend · (Owned labs:GNS3, Vmware, VirtualBox) projects displayed below!
- 📬 Open to: SOC Analyst · Junior Pentester · Blue Team roles

## 🗂️ Lab Projects

### 01 · Network Penetration Testing Lab
Performed a full penetration test lifecycle: reconnaissance, scanning, vulnerability identification, exploitation, and post-exploitation. Documented findings in a structured report format.
- **Tools:** nmap · Metasploit · Hydra
- Target: Metasploitable 2 (192.168.56.XXX)
- ✅ Network scanning with nmap (SYN, version, OS detection)
- ✅ Service enumeration and vulnerability mapping
- ✅ Exploitation via Metasploit Framework
- ✅ Brute force attacks with Hydra

**nmap version scan — identifying vsftpd 2.3.4**
<br><img width="611" height="167" alt="image" src="https://github.com/user-attachments/assets/d51c3811-2c13-4a6e-8a3d-8f0e622d4b43" />

**Metasploit — root shell obtained**
<br><img width="531" height="117" alt="image" src="https://github.com/user-attachments/assets/a8a17a0f-5d3e-42d8-8ba0-347b4e12013e" />
<br><img width="401" height="215" alt="image" src="https://github.com/user-attachments/assets/33cb446c-2d39-4a2c-9f3f-dcbf43f040d4" />


> 📄 **[Download Full Lab Report (PDF)](https://github.com/jaalso/cybersecurity-portfolio/raw/main/Pentest_Lab_Writeup_protected.pdf)**
<br>🔒 Password protected — contact me via [LinkedIn](https://linkedin.com/in/jaalso) to request access

### 02 · Network Traffic Forensics ¦ Phishing Attack Investigation
Scenario: Corporate phishing incident — customer PII exfiltrated to external server
Investigated a real-world-style incident starting from a known outcome ("customer data on Pastebin")
and traced it backwards through a PCAP file to identify the initial intrusion vector, compromised users,
malware delivery chain, and data exfiltration method.
- **Tools:** Wireshark · TShark · VirusTotal · HTTP Object Export
- ✅ Protocol analysis (SMTP analysis — identified spoofed phishing email) (HTTP object export — extracted 26 kB malicious PDF payload from PCAP)
- ✅ PDF forensics — identified embedded JavaScript, auto-execute /OpenAction, obfuscated shellcode
- ✅ VirusTotal analysis — 41/64 engines flagged payload (CVE-2009-0927, CVE-2008-2992)
- ✅ Exfiltration tracing — 1.2 MB of customer PII uploaded to 55.9.19.52 over plain HTTP
- ✅ Attack timeline reconstructed across 5 phases

Key Finding: Two internal victims compromised. Full names, SSNs, credit card numbers and CVVs
exfiltrated in plaintext ~20 hours post-infection. Pastebin filters returned zero results — confirming
exfiltration occurred via direct HTTP upload, not Pastebin directly.

CVEs: CVE-2009-0927 (Adobe Reader JS buffer overflow) · CVE-2008-2992 (util.printf stack overflow)
> 📄 **[Download Full Lab Report (PDF)](https://github.com/jaalso/cybersecurity-portfolio/raw/main/Phishing_Forensics_Writeup_protected.pdf)**
<br>🔒 Password protected — contact me via [LinkedIn](https://linkedin.com/in/jaalso) to request access


### 01 · Home Network Security Audit
Performed a full recon-to-findings audit on a real home network using the same methodology used in
professional penetration tests — ARP sweep, service enumeration, credential testing, and manual verification.
- **Tools:** netdiscover · nmap · Hydra · curl
- Target:  192.168.X.X/24 home gateway.
- ✅ Asset discovery via netdiscover — 10 live hosts identified via ARP sweep (MAC OUI vendor mapping)
- ✅ Full service enumeration — router, IoT devices, etc.
- ✅ Critical finding — unauthenticated admin panel on a Speaker  
- ✅ UPnP enabled on ISP Internet-Box — silent port-opening attack vector identified
- ✅ Hydra false positive analysis — 16 passwords "found" on router, all manually disproved
- ✅ IoT security comparison — Roomba (all ports filtered) vs BeoPlay A9 (5 open, zero auth)
- ✅ Risk assessment with remediation recommendations per finding

Key Finding: Bang & Olufsen Speaker at 192.168.1.XXX exposed a fully
unauthenticated admin panel (GoAhead WebServer) with direct access to network settings and firmware
update capability. SSL certificate expired in 1999 — 26 years ago. 

Notable lesson: Hydra reported 16 valid passwords against the router — all false positives caused by
the router returning identical 301 redirects for every request. Confirmed that automated tool output
must always be manually verified before reporting findings.

**Asset discovery — 10 hosts identified**
<br><img width="553" height="255" alt="image" src="https://github.com/user-attachments/assets/6d4cda6f-b5bc-4c0e-8ece-1498657555d2" />


**Speaker — open ports + expired 1999 SSL cert**
<br><img width="486" height="101" alt="image" src="https://github.com/user-attachments/assets/af662602-c415-4325-8c09-144ddf5b696b" />
<br><img width="468" height="161" alt="image" src="https://github.com/user-attachments/assets/2ead66d0-d467-4ec7-8ba2-4993016ab4eb" />


**Unauthenticated admin panel — direct browser access**
<br><img width="404" height="69" alt="image" src="https://github.com/user-attachments/assets/89f716f6-18d8-4b6e-ba40-82a7f99e7a73" />

> 📄 **[Download Full Lab Report (PDF)](https://github.com/jaalso/cybersecurity-portfolio/raw/main/HomeNetworkAudit_Writeup_protected.pdf)**
<br>🔒 Password protected — contact me via [LinkedIn](https://linkedin.com/in/jaalso) to request access


# 🧰 Tools & Technologies
   Category         Vs           Tools    
- Scanning & Reconnmap ->       Wireshark, TShark, NetworkMiner
- Exploitation    ->            Metasploit, Hydra, CrackMapExec
- Web App Testing   ->          Burp Suite, OWASP ZAP
- SIEM & Monitoring  ->         Wazuh, Elastic Stack, Sysmon
- Email Forensics     ->        emlAnalyzer, CyberChef, MXToolbox
- Phishing Simulation  ->       GoPhish
- Platforms     ->              Kali Linux, Windows 10/11, Metasploitable 2


# 📚 Certifications & Training

- 🎓 Swiss Cyber Institute — Cybersecurity Specialist Program (in progress)
- 🟩 TryHackMe — SOC Level 1 Path (in progress)
 - 📦 HackTheBox — Sherlocks (Blue Team) (in progress)
 - 🛡️ CyberDefenders — Blue Team Labs *(in progress)*


## 🌐 Find Me On
[![TryHackMe](https://img.shields.io/badge/TryHackMe-jaalsove-red?style=for-the-badge&logo=tryhackme)](https://tryhackme.com/p/jaalsove)
[![HackTheBox](https://img.shields.io/badge/HackTheBox-Bornia01-9FEF00?style=for-the-badge&logo=hackthebox&logoColor=black)](https://profile.hackthebox.com/Bornia01)
[![CyberDefenders](https://img.shields.io/badge/CyberDefenders-bornia01-blue?style=for-the-badge)](https://cyberdefenders.org/p/bornia01/)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Jaime%20Soto-0077B5?style=for-the-badge&logo=linkedin)](https://linkedin.com/in/jaalso)

# ⚖️ Legal & Ethical Notice
All penetration testing and offensive security activities documented in this portfolio were conducted exclusively in:

Isolated personal lab environments (VMs with no external connectivity)
Authorized external targets (vuln.land)
Simulated environments provided by training platforms (THM, HTB)

No unauthorized systems were accessed. All work complies with Swiss law and ethical hacking standards.

# Curriculum — Cyber Operations
**Level:** Beginner → Advanced
**Format:** 1 hour per day, fully self-study from home
**Examination:** Each module ends with a practical exam you must complete before moving on

---

## MODULE 1 — Introduction to Cybersecurity

**Description:**
Before you can attack or defend systems you need to understand the fundamentals — what cybersecurity is, how attackers think, and how information is protected. You also learn to break basic ciphers, which is the foundation of all cryptography.

**Prerequisites:** None

**After this module you will be able to:**
- Explain the CIA triad (Confidentiality, Integrity, Availability)
- Describe the difference between ethical and unethical hacking
- Decode and crack Caesar, ROT13, Base64 and hex
- Solve basic CTF challenges on your own

---

### Theory

- [ ] Complete "Intro to Offensive Security" — CIA triad, ethical hacking → **tryhackme.com/room/introtooffensivesecurity**
- [ ] Complete "Security Awareness" — how attackers think → **tryhackme.com/room/securityawarenessintro**
- [ ] Complete the Introduction section — Caesar, ROT13, Base64, hex explained one by one → **cryptohack.org/courses/intro**

### Practice

- [ ] General Skills → "Obedient Cat" → **picoctf.org/practice**
- [ ] General Skills → "Python Wrangling" → **picoctf.org/practice**
- [ ] General Skills → "Wave a flag" → **picoctf.org/practice**
- [ ] Cryptography → "Caesar" → **picoctf.org/practice**
- [ ] Cryptography → "13" (ROT13) → **picoctf.org/practice**
- [ ] Cryptography → "Easy1" (Base64) → **picoctf.org/practice**

### Examination
*Complete these without help. If you get stuck — go back to the theory.*

- [ ] Forensics → "information" → **picoctf.org/practice**
- [ ] Web Exploitation → "Inspect HTML" → **picoctf.org/practice**
- [ ] Web Exploitation → "Don't use client-side" → **picoctf.org/practice**

**✅ MODULE 1 COMPLETE:** 9 picoCTF challenges solved

---

## MODULE 2 — Linux & Networking

**Description:**
Almost all hacking happens through Linux and networks. You need to navigate the terminal without thinking and understand how data actually moves between computers. Without these fundamentals you cannot effectively use a single hacking tool.

**Prerequisites:** Module 1

**After this module you will be able to:**
- Navigate the file system and run commands in a Linux terminal
- Explain how IP addresses, DNS, TCP/UDP and the OSI model work
- Scan open ports on a network using nmap
- Capture and read network traffic in Wireshark

---

### Theory — Linux

- [ ] Complete "Linux Fundamentals Part 1" — file system, basic commands → **tryhackme.com/room/linuxfundamentalspart1**
- [ ] Complete "Linux Fundamentals Part 2" — permissions, processes → **tryhackme.com/room/linuxfundamentalspart2**
- [ ] Complete "Linux Fundamentals Part 3" — scripting, advanced commands → **tryhackme.com/room/linuxfundamentalspart3**

### Theory — Networking

- [ ] Complete "What is Networking?" — IP, MAC addresses → **tryhackme.com/room/whatisnetworking**
- [ ] Complete "DNS in Detail" — how domain names are resolved → **tryhackme.com/room/dnsindetail**
- [ ] Complete "HTTP in Detail" — how web pages are delivered → **tryhackme.com/room/httpindetail**
- [ ] Complete "OSI Model" — the 7 layers → **tryhackme.com/room/osimodelzi**
- [ ] Complete "Packets & Frames" — TCP vs UDP → **tryhackme.com/room/packetsframes**

### Theory — Tools

- [ ] Complete "Nmap" — how to scan networks → **tryhackme.com/room/furthernmap**
- [ ] Complete "Wireshark: The Basics" — how to read traffic → **tryhackme.com/room/wiresharkthebasics**

### Examination
*Complete these without help. They require combining Linux and networking knowledge.*

- [ ] Forensics → "Wireshark doo dooo do doo" → **picoctf.org/practice**
- [ ] Forensics → "Packet Primo" → **picoctf.org/practice**
- [ ] Reach a total of 20 solved picoCTF challenges → **picoctf.org/practice**

**✅ MODULE 2 COMPLETE:** Linux + networking + 20 picoCTF

---

## MODULE 3 — Web Attacks

**Description:**
The web is the most common attack surface. You learn how the most widely used attacks work — SQL injection, XSS and authentication attacks — and execute them against real labs. Everything is based on the OWASP Top 10, the industry standard for web security.

**Prerequisites:** Module 2

**After this module you will be able to:**
- Perform SQL injection and log in without a password
- Inject and execute XSS code in a web page
- Crack weak authentication with brute force
- Identify and explain OWASP Top 10 vulnerabilities

---

### Theory — SQL Injection

- [ ] Read the theory on how databases are attacked → **portswigger.net/web-security/sql-injection**

### Practice — SQL Injection

- [ ] Complete lab "retrieve-hidden-data" — extract hidden data → **portswigger.net/web-security/sql-injection/lab-retrieve-hidden-data**
- [ ] Complete lab "login-bypass" — log in without a password → **portswigger.net/web-security/sql-injection/lab-login-bypass**

### Theory — XSS

- [ ] Read the theory on how JavaScript is injected → **portswigger.net/web-security/cross-site-scripting**

### Practice — XSS

- [ ] Complete lab "reflected XSS" → **portswigger.net/web-security/cross-site-scripting/reflected/lab-html-context-nothing-encoded**
- [ ] Complete lab "stored XSS" → **portswigger.net/web-security/cross-site-scripting/stored/lab-html-context-nothing-encoded**

### Theory — Authentication & CSRF

- [ ] Read the theory on authentication attacks → **portswigger.net/web-security/authentication**
- [ ] Read the theory on CSRF → **portswigger.net/web-security/csrf**

### Practice — Authentication & CSRF

- [ ] Complete 2 authentication labs → **portswigger.net/web-security/authentication/password-based**
- [ ] Complete 1 CSRF lab → **portswigger.net/web-security/csrf**

### Examination
*Complete these without help and write a writeup for one of them.*

- [ ] Web Exploitation → "SQL Direct" → **picoctf.org/practice**
- [ ] Web Exploitation → "Cookies" → **picoctf.org/practice**
- [ ] Web Exploitation → "More Cookies" → **picoctf.org/practice**
- [ ] Reach a total of 30 solved picoCTF challenges → **picoctf.org/practice**
- [ ] Write 1 writeup → [ctf-writeups/picoctf/mall.md](ctf-writeups/picoctf/mall.md)

**✅ MODULE 3 COMPLETE:** 10 PortSwigger labs + 30 picoCTF + writeup

---

## MODULE 4 — OSINT

**Description:**
Before an attacker touches a system they gather information — openly and passively, without leaving a trace. You learn how to map a target using only open-source information: Google, metadata, images and internet-exposed devices.

**Prerequisites:** Module 2

**After this module you will be able to:**
- Gather information about a target without contacting it
- Use Google Dorking to find exposed files and directories
- Discover exposed devices and services using Shodan
- Analyze images to determine where they were taken

---

### Theory

- [ ] Complete "Google Dorking" — find sensitive info via Google → **tryhackme.com/room/googledorking**
- [ ] Complete "Shodan" — map exposed devices → **tryhackme.com/room/shodan**

### Examination
*Complete these on your own — they test if you can combine OSINT techniques.*

- [ ] Complete "OhSINT" — find everything about a person from a single image → **tryhackme.com/room/ohsint**
- [ ] Complete "Searchlight - IMINT" — geolocate an image → **tryhackme.com/room/searchlightosint**
- [ ] Forensics → "Trivial Flag Transfer Protocol" → **picoctf.org/practice**
- [ ] Forensics → "Enhance!" → **picoctf.org/practice**
- [ ] Forensics → "Sleuthkit Intro" → **picoctf.org/practice**

**✅ MODULE 4 COMPLETE:** OSINT + passive reconnaissance + 3 forensics

---

## MODULE 5 — Log Analysis & Incident Response

**Description:**
A cyber operator must be able to read logs and identify intrusions. You learn to follow an attack step by step through log data — from first contact to full compromise — and how to set up systems that automatically alert on suspicious traffic.

**Prerequisites:** Module 2 and 3

**After this module you will be able to:**
- Read and understand Windows and Linux system logs
- Identify an ongoing intrusion in log data
- Use Splunk to search and analyze logs
- Configure Snort to detect attacks in network traffic

---

### Theory — Logs

- [ ] Complete "Windows Event Logs" — understand Windows logs → **tryhackme.com/room/windowseventlogs**
- [ ] Complete "Linux Forensics" — understand Linux logs → **tryhackme.com/room/linuxforensics**
- [ ] Complete "Splunk: Basics" — learn the log analysis tool → **tryhackme.com/room/splunk101**
- [ ] Complete "Snort" — intrusion detection → **tryhackme.com/room/snort**

### Examination
*Complete these on your own. You must find a real attack in log data.*

- [ ] Complete "Investigating with Splunk" — find an attack in real log data → **tryhackme.com/room/investigatingwithsplunk**
- [ ] Complete "Traffic Analysis Essentials" → **tryhackme.com/room/trafficanalysisessentials**
- [ ] Complete "Incident Response and Forensics" → **tryhackme.com/room/incidentresponseintro**
- [ ] Forensics → "Operation Oni" → **picoctf.org/practice**
- [ ] Forensics → "Eavesdrop" → **picoctf.org/practice**
- [ ] Reach a total of 40 solved picoCTF challenges → **picoctf.org/practice**

**✅ MODULE 5 COMPLETE:** Log analysis + IDS + 40 picoCTF

---

## MODULE 6 — Attack Techniques & Penetration Testing

**Description:**
Now you combine everything you have learned and attack real systems. You learn the full penetration testing methodology — from reconnaissance to exploitation to becoming admin — and automate parts of the work with Python.

**Prerequisites:** Module 2, 3 and 5

**After this module you will be able to:**
- Conduct a full penetration test (recon → exploit → root)
- Escalate privileges from regular user to admin/root
- Use Metasploit to exploit known vulnerabilities
- Write your own attack scripts in Python

---

### Theory

- [ ] Complete "Metasploit: Introduction" — learn the framework → **tryhackme.com/room/metasploitintro**
- [ ] Complete "Privilege Escalation" — learn to become admin → **tryhackme.com/room/privescpending**
- [ ] Complete "Hello World" through "Functions" — Python basics → **learnpython.org**

### Practice

- [ ] Complete "Blue" — exploit Windows with Metasploit → **tryhackme.com/room/blue**
- [ ] Complete "Ice" — full Windows exploitation → **tryhackme.com/room/ice**

### Examination
*Complete these without a walkthrough. Write a writeup for each.*

- [ ] Starting Point → "Meow" — Telnet → **hackthebox.com/starting-point**
- [ ] Starting Point → "Fawn" — FTP → **hackthebox.com/starting-point**
- [ ] Starting Point → "Dancing" — SMB → **hackthebox.com/starting-point**
- [ ] Starting Point → "Redeemer" — Redis → **hackthebox.com/starting-point**
- [ ] Starting Point → "Explosion" — RDP → **hackthebox.com/starting-point**
- [ ] Machines → complete 5 Easy machines → **hackthebox.com/machines**
- [ ] Write a writeup for each machine → [ctf-writeups/hackthebox/mall.md](ctf-writeups/hackthebox/mall.md)
- [ ] Write your own port-scanning script in Python → [notes/verktyg/cheatsheet.md](notes/verktyg/cheatsheet.md)

**✅ MODULE 6 COMPLETE:** 10 HTB machines + writeups + Python script

---

## MODULE 7 — Live CTF & Advanced

**Description:**
Final module. You now compete against real people under time pressure and prove you can solve unknown problems on your own. You also build a complete portfolio documenting your entire journey.

**Prerequisites:** Modules 1–6

**After this module you will be able to:**
- Solve unknown CTF challenges under time pressure
- Explain and document your solutions in writeups
- Conduct Red Team operations
- Present a portfolio demonstrating your technical competence

---

### Theory — Advanced

- [ ] Complete the full "Junior Penetration Tester" path → **tryhackme.com/path/outline/jrpenetrationtester**
- [ ] Complete "Red Team Fundamentals" → **tryhackme.com/room/redteamfundamentals**
- [ ] Complete "Red Team Recon" → **tryhackme.com/room/redteamrecon**

### Examination — Live Competition

- [ ] Compete in the picoCTF live event (held every March) → **picoctf.org**
- [ ] Solve at least 10 challenges in the live event
- [ ] Find and enter an external CTF → **ctftime.org**
- [ ] Solve at least 5 challenges in the external CTF
- [ ] Reach rank "Hacker" on HackTheBox → **hackthebox.com**
- [ ] Have at least 10 writeups published in this repo → [ctf-writeups/](ctf-writeups/)

**✅ MODULE 7 COMPLETE:** Ready for cyber operations

---

## Total Progress
- picoCTF challenges: 0 / 40+
- PortSwigger labs: 0 / 10
- TryHackMe rooms: 0 / 20+
- HackTheBox machines: 0 / 10+
- Writeups: 0 / 10+

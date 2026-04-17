# Roadmap — Cybersoldat
Uppdatera [ ] till [x] när du är klar.

---

## FAS 1 — Absoluta grunder

**Mål:**
- Förstå vad cybersäkerhet, etisk hacking och CIA-triaden är
- Knäcka enkla chiffer (Caesar, Base64, ROT13, hex)
- Lösa dina första CTF-utmaningar helt på egen hand

- [ ] FAS 1 klar

---

### Lär dig — Etisk hacking & CIA-triaden

- [ ] Klara "Intro to Offensive Security" → **tryhackme.com/room/introtooffensivesecurity**
- [ ] Klara "Security Awareness" → **tryhackme.com/room/securityawarenessintro**

### Lär dig — Caesar, ROT13, Base64, Hex

- [ ] Klara alla 7 utmaningar i "Introduction" — varje utmaning lär dig ett nytt chiffer → **cryptohack.org/courses/intro**

### Testa & Visa — Lösa CTF på egen hand

- [ ] General Skills → "Obedient Cat" → **picoctf.org/practice**
- [ ] General Skills → "Python Wrangling" → **picoctf.org/practice**
- [ ] General Skills → "Wave a flag" → **picoctf.org/practice**
- [ ] Cryptography → "Caesar" → **picoctf.org/practice**
- [ ] Cryptography → "13" (ROT13) → **picoctf.org/practice**
- [ ] Cryptography → "Easy1" (Base64) → **picoctf.org/practice**
- [ ] Forensics → "information" → **picoctf.org/practice**
- [ ] Web Exploitation → "Inspect HTML" → **picoctf.org/practice**
- [ ] Web Exploitation → "Don't use client-side" → **picoctf.org/practice**

**✅ DELMÅL 1:** 9 picoCTF lösta + grundförståelse för cybersäkerhet

---

## FAS 2 — Linux & Nätverk

**Mål:**
- Navigera och köra kommandon i Linux utan att googla
- Förstå hur IP, DNS, TCP/UDP, HTTP och OSI-modellen fungerar
- Skanna ett nätverk med nmap och analysera trafik i Wireshark

- [ ] FAS 2 klar

---

### Lär dig — Linux

- [ ] Klara "Linux Fundamentals Part 1" → **tryhackme.com/room/linuxfundamentalspart1**
- [ ] Klara "Linux Fundamentals Part 2" → **tryhackme.com/room/linuxfundamentalspart2**
- [ ] Klara "Linux Fundamentals Part 3" → **tryhackme.com/room/linuxfundamentalspart3**

### Lär dig — Nätverk

- [ ] Klara "What is Networking?" — IP, MAC → **tryhackme.com/room/whatisnetworking**
- [ ] Klara "DNS in Detail" → **tryhackme.com/room/dnsindetail**
- [ ] Klara "HTTP in Detail" → **tryhackme.com/room/httpindetail**
- [ ] Klara "OSI Model" → **tryhackme.com/room/osimodelzi**
- [ ] Klara "Packets & Frames" — TCP vs UDP → **tryhackme.com/room/packetsframes**

### Lär dig — Verktyg

- [ ] Klara "Nmap" — port scanning → **tryhackme.com/room/furthernmap**
- [ ] Klara "Wireshark: The Basics" → **tryhackme.com/room/wiresharkthebasics**

### Testa & Visa — Nätverksanalys i CTF

- [ ] Forensics → "Wireshark doo dooo do doo" → **picoctf.org/practice**
- [ ] Forensics → "Packet Primo" → **picoctf.org/practice**
- [ ] Totalt 20 lösta picoCTF utmaningar → **picoctf.org/practice**

**✅ DELMÅL 2:** Linux + nätverk + verktyg + 20 picoCTF

---

## FAS 3 — Webbattacker

**Mål:**
- Utföra SQL injection och ta sig förbi en inloggning
- Injicera XSS-kod i en webbsida
- Förstå och förklara OWASP Top 10

- [ ] FAS 3 klar

---

### Lär dig — SQL Injection

- [ ] Läs teorin → **portswigger.net/web-security/sql-injection**

### Testa & Visa — SQL Injection

- [ ] Klara lab "retrieve-hidden-data" → **portswigger.net/web-security/sql-injection/lab-retrieve-hidden-data**
- [ ] Klara lab "login-bypass" → **portswigger.net/web-security/sql-injection/lab-login-bypass**
- [ ] Web Exploitation → lös "SQL Direct" → **picoctf.org/practice**

### Lär dig — XSS

- [ ] Läs teorin → **portswigger.net/web-security/cross-site-scripting**

### Testa & Visa — XSS

- [ ] Klara lab "reflected XSS" → **portswigger.net/web-security/cross-site-scripting/reflected/lab-html-context-nothing-encoded**
- [ ] Klara lab "stored XSS" → **portswigger.net/web-security/cross-site-scripting/stored/lab-html-context-nothing-encoded**

### Lär dig — Autentiseringsattacker

- [ ] Läs teorin → **portswigger.net/web-security/authentication**

### Testa & Visa — Autentisering & CSRF

- [ ] Klara 2 authentication-labbar → **portswigger.net/web-security/authentication/password-based**
- [ ] Klara 1 CSRF-labb → **portswigger.net/web-security/csrf**
- [ ] Web Exploitation → lös "Cookies" → **picoctf.org/practice**
- [ ] Web Exploitation → lös "More Cookies" → **picoctf.org/practice**
- [ ] Totalt 30 lösta picoCTF utmaningar → **picoctf.org/practice**
- [ ] Skriv 1 writeup → [ctf-writeups/picoctf/mall.md](ctf-writeups/picoctf/mall.md)

**✅ DELMÅL 3:** 10 PortSwigger-labbar + 30 picoCTF + writeup

---

## FAS 4 — OSINT

**Mål:**
- Samla information om ett mål utan att röra det
- Hitta subdomäner, exponerade filer och läckta uppgifter
- Förstå hur angripare använder öppen information som vapen

- [ ] FAS 4 klar

---

### Lär dig — OSINT-tekniker

- [ ] Klara "Google Dorking" — avancerade sökningar → **tryhackme.com/room/googledorking**
- [ ] Klara "Shodan" — hitta exponerade enheter → **tryhackme.com/room/shodan**

### Testa & Visa — OSINT i praktiken

- [ ] Klara "OhSINT" — hitta info om en person med bara en bild → **tryhackme.com/room/ohsint**
- [ ] Klara "Searchlight - IMINT" — bildanalys, geolokalisering → **tryhackme.com/room/searchlightosint**
- [ ] Forensics → lös "Trivial Flag Transfer Protocol" → **picoctf.org/practice**
- [ ] Forensics → lös "Enhance!" → **picoctf.org/practice**
- [ ] Forensics → lös "Sleuthkit Intro" → **picoctf.org/practice**

**✅ DELMÅL 4:** OSINT + passiv spaning + 3 forensics picoCTF

---

## FAS 5 — Logganalys & Incidenthantering

**Mål:**
- Läsa och förstå systemloggar och nätverksloggar
- Identifiera ett pågående intrång i loggar
- Följa ett angrepp från start till slut i loggdata

- [ ] FAS 5 klar

---

### Lär dig — Loggar

- [ ] Klara "Windows Event Logs" → **tryhackme.com/room/windowseventlogs**
- [ ] Klara "Linux Forensics" → **tryhackme.com/room/linuxforensics**
- [ ] Klara "Splunk: Basics" → **tryhackme.com/room/splunk101**
- [ ] Klara "Snort" — intrångsdetektering → **tryhackme.com/room/snort**

### Testa & Visa — Hitta angrepp i loggar

- [ ] Klara "Investigating with Splunk" — hitta ett riktigt angrepp i loggar → **tryhackme.com/room/investigatingwithsplunk**
- [ ] Klara "Traffic Analysis Essentials" → **tryhackme.com/room/trafficanalysisessentials**
- [ ] Klara "Incident Response and Forensics" → **tryhackme.com/room/incidentresponseintro**
- [ ] Forensics → lös "Operation Oni" → **picoctf.org/practice**
- [ ] Forensics → lös "Eavesdrop" → **picoctf.org/practice**
- [ ] Totalt 40 lösta picoCTF utmaningar → **picoctf.org/practice**

**✅ DELMÅL 5:** Logganalys + IDS + 40 picoCTF

---

## FAS 6 — Attacktekniker & Penetrationstestning

**Mål:**
- Ta dig in i en riktig maskin från scratch (recon → exploit → root)
- Eskalera rättigheter från användare till admin/root
- Använda Metasploit och skriva egna attack-scripts i Python

- [ ] FAS 6 klar

---

### Lär dig — Attackverktyg

- [ ] Klara "Metasploit: Introduction" → **tryhackme.com/room/metasploitintro**
- [ ] Klara "Privilege Escalation" → **tryhackme.com/room/privescpending**
- [ ] Klara "Hello World" till "Functions" → **learnpython.org**

### Testa & Visa — Hacka riktiga maskiner

- [ ] Klara "Blue" — exploatera Windows med Metasploit → **tryhackme.com/room/blue**
- [ ] Klara "Ice" — Windows exploitation → **tryhackme.com/room/ice**
- [ ] Starting Point → klara "Meow" — Telnet → **hackthebox.com/starting-point**
- [ ] Starting Point → klara "Fawn" — FTP → **hackthebox.com/starting-point**
- [ ] Starting Point → klara "Dancing" — SMB → **hackthebox.com/starting-point**
- [ ] Starting Point → klara "Redeemer" — Redis → **hackthebox.com/starting-point**
- [ ] Starting Point → klara "Explosion" — RDP → **hackthebox.com/starting-point**
- [ ] Machines → klara 5 Easy-maskiner → **hackthebox.com/machines**
- [ ] Skriv writeup för varje maskin → [ctf-writeups/hackthebox/mall.md](ctf-writeups/hackthebox/mall.md)
- [ ] Skriv ett eget port-scanning script → [notes/verktyg/cheatsheet.md](notes/verktyg/cheatsheet.md)

**✅ DELMÅL 6:** 10 HTB-maskiner + writeups + Python-script

---

## FAS 7 — Live CTF & Portfolio

**Mål:**
- Tävla mot andra under tidspress i live CTF
- Ha ett komplett portfolio med writeups
- Vara tekniskt redo för cyberoperationer

- [ ] FAS 7 klar

---

### Lär dig — Avancerat

- [ ] Klara hela "Junior Penetration Tester"-pathen → **tryhackme.com/path/outline/jrpenetrationtester**
- [ ] Klara "Red Team Fundamentals" → **tryhackme.com/room/redteamfundamentals**
- [ ] Klara "Red Team Recon" → **tryhackme.com/room/redteamrecon**

### Testa & Visa — Tävla live

- [ ] Delta i live-tävlingen (mars varje år) → **picoctf.org**
- [ ] Lös minst 10 utmaningar i live-tävlingen → **picoctf.org**
- [ ] Hitta en extern CTF → delta → **ctftime.org**
- [ ] Lös minst 5 utmaningar i extern CTF → **ctftime.org**
- [ ] Nå rank "Hacker" (~20 lösta maskiner) → **hackthebox.com**
- [ ] Ha minst 10 writeups i repot → [ctf-writeups/](ctf-writeups/)

**✅ DELMÅL 7:** Tekniskt redo för cyberoperationer

---

## Totalt framsteg
- picoCTF utmaningar: 0 / 40+
- PortSwigger labbar: 0 / 10
- TryHackMe rum: 0 / 20+
- HackTheBox maskiner: 0 / 10+
- Writeups: 0 / 10+

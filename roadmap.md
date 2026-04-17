# Roadmap — Cybersoldat
Uppdatera [ ] till [x] när du är klar.

---

## FAS 1 — Absoluta grunder

**Mål:**
- Förstå vad cybersäkerhet, etisk hacking och CIA-triaden är
- Knäcka enkla chiffer (Caesar, Base64, ROT13, hex)
- Lösa dina första CTF-utmaningar helt på egen hand

**Genomfört:**
- [ ] FAS 1 klar

---

### TryHackMe
Lär dig här: **tryhackme.com**

- [ ] Klara "Intro to Offensive Security" — vad etisk hacking är, CIA-triaden
- [ ] Klara "Security Awareness" — hur angripare tänker

### CryptoHack
Lär dig här: **cryptohack.org → Introduction**

- [ ] Klara alla 7 utmaningar i Introduction-sektionen

### picoCTF
Lär dig här: **picoctf.org → Practice**

- [ ] General Skills → "Obedient Cat"
- [ ] General Skills → "Python Wrangling"
- [ ] General Skills → "Wave a flag"
- [ ] Cryptography → "Caesar"
- [ ] Cryptography → "13" (ROT13)
- [ ] Cryptography → "Easy1"
- [ ] Forensics → "information"
- [ ] Web Exploitation → "Inspect HTML"
- [ ] Web Exploitation → "Don't use client-side"

**✅ DELMÅL 1:** Grundförståelse för cybersäkerhet + 9 picoCTF lösta

---

## FAS 2 — Linux & Nätverk

**Mål:**
- Navigera och köra kommandon i Linux utan att googla
- Förstå hur IP, DNS, TCP/UDP, HTTP och OSI-modellen fungerar
- Skanna ett nätverk med nmap och analysera trafik i Wireshark

**Genomfört:**
- [ ] FAS 2 klar

---

### TryHackMe — Linux
Lär dig här: **tryhackme.com**

- [ ] Klara "Linux Fundamentals Part 1"
- [ ] Klara "Linux Fundamentals Part 2"
- [ ] Klara "Linux Fundamentals Part 3"

### TryHackMe — Nätverk
Lär dig här: **tryhackme.com**

- [ ] Klara "What is Networking?" — IP-adresser, MAC
- [ ] Klara "DNS in Detail" — hur DNS fungerar
- [ ] Klara "HTTP in Detail" — hur webb fungerar
- [ ] Klara "OSI Model" — de 7 lagren
- [ ] Klara "Packets & Frames" — TCP vs UDP

### TryHackMe — Verktyg
Lär dig här: **tryhackme.com**

- [ ] Klara "Nmap" — port scanning
- [ ] Klara "Wireshark: The Basics" — nätverksanalys

### picoCTF
Lär dig här: **picoctf.org → Practice**

- [ ] Forensics → "Wireshark doo dooo do doo"
- [ ] Forensics → "Packet Primo"
- [ ] Totalt 20 lösta utmaningar

**✅ DELMÅL 2:** Linux-kompetens + nätverk + verktyg + 20 picoCTF

---

## FAS 3 — Webbattacker

**Mål:**
- Utföra SQL injection och ta sig förbi en inloggning
- Injicera XSS-kod i en webbsida
- Förstå och förklara OWASP Top 10

**Genomfört:**
- [ ] FAS 3 klar

---

### PortSwigger — SQL Injection
Lär dig här: **portswigger.net/web-security/sql-injection**

- [ ] Läs teorin
- [ ] Klara lab "retrieve-hidden-data"
- [ ] Klara lab "login-bypass"

### PortSwigger — XSS
Lär dig här: **portswigger.net/web-security/cross-site-scripting**

- [ ] Läs teorin
- [ ] Klara lab "reflected/lab-html-context-nothing-encoded"
- [ ] Klara lab "stored/lab-html-context-nothing-encoded"

### PortSwigger — Autentisering
Lär dig här: **portswigger.net/web-security/authentication**

- [ ] Läs teorin
- [ ] Klara 2 labbar

### PortSwigger — CSRF
Lär dig här: **portswigger.net/web-security/csrf**

- [ ] Läs teorin
- [ ] Klara 1 labb

### picoCTF
Lär dig här: **picoctf.org → Practice → Web Exploitation**

- [ ] Lös "SQL Direct"
- [ ] Lös "Cookies"
- [ ] Lös "More Cookies"
- [ ] Totalt 30 lösta utmaningar

### Writeup
- [ ] Skriv 1 writeup om en webbattack → [ctf-writeups/picoctf/mall.md](ctf-writeups/picoctf/mall.md)

**✅ DELMÅL 3:** 10 PortSwigger-labbar + 30 picoCTF + writeup

---

## FAS 4 — OSINT

**Mål:**
- Samla information om ett mål utan att röra det (passiv spaning)
- Hitta subdomäner, exponerade filer och läckta uppgifter
- Förstå hur angripare använder öppen information som vapen

**Genomfört:**
- [ ] FAS 4 klar

---

### TryHackMe — OSINT
Lär dig här: **tryhackme.com**

- [ ] Klara "OSINT" rummet
- [ ] Klara "Google Dorking" — avancerade Google-sökningar
- [ ] Klara "Searchlight - IMINT" — bildanalys och geolokalisering

### Verktyg att lära sig
Lär dig här: **tryhackme.com → sök på respektive verktyg**

- [ ] Klara "Shodan" — hitta exponerade enheter på internet
- [ ] Klara "Intro to OSINT" — metadata, sociala medier, domäninfo

### picoCTF
Lär dig här: **picoctf.org → Practice → Forensics**

- [ ] Lös "Trivial Flag Transfer Protocol"
- [ ] Lös "Enhance!"
- [ ] Lös "Sleuthkit Intro"

**✅ DELMÅL 4:** OSINT-verktyg + passiv spaning + 3 picoCTF forensics

---

## FAS 5 — Logganalys & Incidenthantering

**Mål:**
- Läsa och förstå systemloggar och nätverksloggar
- Identifiera ett pågående intrång i loggar
- Följa ett angrepp från start till slut i loggdata

**Genomfört:**
- [ ] FAS 5 klar

---

### TryHackMe — Loggar & SOC
Lär dig här: **tryhackme.com**

- [ ] Klara "Incident Response and Forensics"
- [ ] Klara "Windows Event Logs" — läsa Windows-loggar
- [ ] Klara "Linux Forensics" — läsa Linux-loggar
- [ ] Klara "Splunk: Basics" — logganalysverktyg
- [ ] Klara "Investigating with Splunk" — hitta angrepp i loggar

### TryHackMe — Nätverksdetektering
Lär dig här: **tryhackme.com**

- [ ] Klara "Snort" — intrångsdetektering (IDS)
- [ ] Klara "Traffic Analysis Essentials"

### picoCTF
Lär dig här: **picoctf.org → Practice → Forensics**

- [ ] Lös "Operation Oni"
- [ ] Lös "Eavesdrop"
- [ ] Totalt 40 lösta utmaningar

**✅ DELMÅL 5:** Logganalys + IDS + 40 picoCTF

---

## FAS 6 — Attacktekniker & Penetrationstestning

**Mål:**
- Ta dig in i en riktig maskin från scratch (recon → exploit → root)
- Eskalera rättigheter från användare till admin/root
- Förstå och använda verktyg som Metasploit och Burp Suite

**Genomfört:**
- [ ] FAS 6 klar

---

### TryHackMe — Pentesting
Lär dig här: **tryhackme.com**

- [ ] Klara "Metasploit: Introduction"
- [ ] Klara "Blue" — exploatera en riktig Windows-maskin
- [ ] Klara "Ice" — Windows exploitation
- [ ] Klara "Privilege Escalation" rummet

### HackTheBox — Starting Point
Lär dig här: **hackthebox.com → Starting Point**

- [ ] Klara "Meow" — grundläggande Telnet
- [ ] Klara "Fawn" — FTP-attack
- [ ] Klara "Dancing" — SMB-attack
- [ ] Klara "Redeemer" — Redis-attack
- [ ] Klara "Explosion" — RDP-attack

### HackTheBox — Easy maskiner
Lär dig här: **hackthebox.com → Machines → Easy**

- [ ] Klara 5 Easy-maskiner
- [ ] Skriv writeup för varje maskin → [ctf-writeups/hackthebox/mall.md](ctf-writeups/hackthebox/mall.md)

### Python — Automatisera attacker
Lär dig här: **learnpython.org**

- [ ] Klara "Hello World" till "Functions"
- [ ] Skriv ett port-scanning script → se [notes/verktyg/cheatsheet.md](notes/verktyg/cheatsheet.md)
- [ ] Skriv ett script som automatiserar en attack du lärt dig

**✅ DELMÅL 6:** 10 HTB-maskiner + writeups + eget attack-script

---

## FAS 7 — Live CTF & Portfolio

**Mål:**
- Tävla mot andra under tidspress i live CTF
- Ha ett komplett portfolio med writeups
- Vara tekniskt redo för cyberoperationer

**Genomfört:**
- [ ] FAS 7 klar

---

### picoCTF — Live tävling
Lär dig här: **picoctf.org** (tävling varje år i mars)

- [ ] Delta i live-tävlingen
- [ ] Lös minst 10 utmaningar
- [ ] Skriv writeup för varje lösning

### CTFtime — Andra tävlingar
Lär dig här: **ctftime.org**

- [ ] Hitta en kommande CTF → delta
- [ ] Lös minst 5 utmaningar
- [ ] Skriv writeups

### TryHackMe — Avancerat
Lär dig här: **tryhackme.com**

- [ ] Klara hela "Junior Penetration Tester"-pathen
- [ ] Klara "Red Team Fundamentals"
- [ ] Klara "Red Team Recon"

### HackTheBox — Rank upp
Lär dig här: **hackthebox.com**

- [ ] Nå rank "Hacker" (~20 lösta maskiner totalt)

**✅ DELMÅL 7:** Tekniskt redo för cyberoperationer

---

## Totalt framsteg
- picoCTF utmaningar: 0 / 40+
- PortSwigger labbar: 0 / 10
- TryHackMe rum: 0 / 20+
- HackTheBox maskiner: 0 / 10+
- Writeups: 0 / 10+

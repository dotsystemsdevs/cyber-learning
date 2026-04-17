# Kursplan — Cybersoldat
**Nivå:** Nybörjare → Avancerad
**Upplägg:** 1 timme per dag, självstudier hemifrån
**Examination:** Varje modul avslutas med ett praktiskt prov du måste klara

---

## MODUL 1 — Introduktion till Cybersäkerhet

**Beskrivning:**
Innan du kan attackera eller försvara system måste du förstå grunderna — vad cybersäkerhet är, hur angripare tänker och hur information skyddas. Du lär dig också att knäcka enkla chiffer, vilket är grunden för all kryptografi.

**Förkunskapskrav:** Inga

**Efter denna modul kan du:**
- Förklara CIA-triaden (Konfidentialitet, Integritet, Tillgänglighet)
- Beskriva skillnaden mellan etisk och oetisk hacking
- Avkoda och knäcka Caesar, ROT13, Base64 och hex
- Lösa enkla CTF-utmaningar på egen hand

---

### Teori

- [ ] Klara "Intro to Offensive Security" — CIA-triaden, etisk hacking → **tryhackme.com/room/introtooffensivesecurity**
- [ ] Klara "Security Awareness" — hur angripare tänker → **tryhackme.com/room/securityawarenessintro**
- [ ] Klara Introduction-sektionen — Caesar, ROT13, Base64, hex förklaras ett i taget → **cryptohack.org/courses/intro**

### Praktik

- [ ] General Skills → "Obedient Cat" → **picoctf.org/practice**
- [ ] General Skills → "Python Wrangling" → **picoctf.org/practice**
- [ ] General Skills → "Wave a flag" → **picoctf.org/practice**
- [ ] Cryptography → "Caesar" → **picoctf.org/practice**
- [ ] Cryptography → "13" (ROT13) → **picoctf.org/practice**
- [ ] Cryptography → "Easy1" (Base64) → **picoctf.org/practice**

### Examination
*Klara dessa utan hjälp. Om du fastnar — gå tillbaka till teorin.*

- [ ] Forensics → "information" → **picoctf.org/practice**
- [ ] Web Exploitation → "Inspect HTML" → **picoctf.org/practice**
- [ ] Web Exploitation → "Don't use client-side" → **picoctf.org/practice**

**✅ MODUL 1 GODKÄND:** 9 picoCTF lösta

---

## MODUL 2 — Linux & Nätverk

**Beskrivning:**
Nästan all hacking sker via Linux och nätverk. Du måste kunna terminalen utan att tänka och förstå hur data faktiskt rör sig mellan datorer. Utan dessa grunder kan du inte använda ett enda hackning-verktyg effektivt.

**Förkunskapskrav:** Modul 1

**Efter denna modul kan du:**
- Navigera filsystemet och köra kommandon i Linux-terminalen
- Förklara hur IP-adresser, DNS, TCP/UDP och OSI-modellen fungerar
- Skanna öppna portar på ett nätverk med nmap
- Fånga och läsa nätverkstrafik i Wireshark

---

### Teori — Linux

- [ ] Klara "Linux Fundamentals Part 1" — filsystem, grundkommandon → **tryhackme.com/room/linuxfundamentalspart1**
- [ ] Klara "Linux Fundamentals Part 2" — rättigheter, processer → **tryhackme.com/room/linuxfundamentalspart2**
- [ ] Klara "Linux Fundamentals Part 3" — scripting, avancerade kommandon → **tryhackme.com/room/linuxfundamentalspart3**

### Teori — Nätverk

- [ ] Klara "What is Networking?" — IP, MAC-adresser → **tryhackme.com/room/whatisnetworking**
- [ ] Klara "DNS in Detail" — hur domännamn översätts → **tryhackme.com/room/dnsindetail**
- [ ] Klara "HTTP in Detail" — hur webbsidor skickas → **tryhackme.com/room/httpindetail**
- [ ] Klara "OSI Model" — de 7 lagren → **tryhackme.com/room/osimodelzi**
- [ ] Klara "Packets & Frames" — TCP vs UDP → **tryhackme.com/room/packetsframes**

### Teori — Verktyg

- [ ] Klara "Nmap" — hur du skannar nätverk → **tryhackme.com/room/furthernmap**
- [ ] Klara "Wireshark: The Basics" — hur du läser trafik → **tryhackme.com/room/wiresharkthebasics**

### Examination
*Klara dessa utan hjälp. De kräver att du kombinerar Linux och nätverkskunskap.*

- [ ] Forensics → "Wireshark doo dooo do doo" → **picoctf.org/practice**
- [ ] Forensics → "Packet Primo" → **picoctf.org/practice**
- [ ] Totalt 20 lösta picoCTF utmaningar → **picoctf.org/practice**

**✅ MODUL 2 GODKÄND:** Linux + nätverk + 20 picoCTF

---

## MODUL 3 — Webbattacker

**Beskrivning:**
Webb är den vanligaste attackytan. Du lär dig hur de mest använda attackerna fungerar — SQL injection, XSS och autentiseringsattacker — och utför dem mot riktiga labbar. Allt baseras på OWASP Top 10, branschstandarden för webbsäkerhet.

**Förkunskapskrav:** Modul 2

**Efter denna modul kan du:**
- Utföra SQL injection och logga in utan lösenord
- Injicera och köra XSS-kod i en webbsida
- Knäcka svag autentisering med brute force
- Förklara och identifiera OWASP Top 10-sårbarheter

---

### Teori — SQL Injection

- [ ] Läs teorin om hur databaser attackeras → **portswigger.net/web-security/sql-injection**

### Praktik — SQL Injection

- [ ] Klara lab "retrieve-hidden-data" — hämta dold data → **portswigger.net/web-security/sql-injection/lab-retrieve-hidden-data**
- [ ] Klara lab "login-bypass" — logga in utan lösenord → **portswigger.net/web-security/sql-injection/lab-login-bypass**

### Teori — XSS

- [ ] Läs teorin om hur JavaScript injiceras → **portswigger.net/web-security/cross-site-scripting**

### Praktik — XSS

- [ ] Klara lab "reflected XSS" → **portswigger.net/web-security/cross-site-scripting/reflected/lab-html-context-nothing-encoded**
- [ ] Klara lab "stored XSS" → **portswigger.net/web-security/cross-site-scripting/stored/lab-html-context-nothing-encoded**

### Teori — Autentisering & CSRF

- [ ] Läs teorin om autentiseringsattacker → **portswigger.net/web-security/authentication**
- [ ] Läs teorin om CSRF → **portswigger.net/web-security/csrf**

### Praktik — Autentisering & CSRF

- [ ] Klara 2 authentication-labbar → **portswigger.net/web-security/authentication/password-based**
- [ ] Klara 1 CSRF-labb → **portswigger.net/web-security/csrf**

### Examination
*Klara dessa utan hjälp och skriv en writeup om en av dem.*

- [ ] Web Exploitation → "SQL Direct" → **picoctf.org/practice**
- [ ] Web Exploitation → "Cookies" → **picoctf.org/practice**
- [ ] Web Exploitation → "More Cookies" → **picoctf.org/practice**
- [ ] Totalt 30 lösta picoCTF utmaningar → **picoctf.org/practice**
- [ ] Skriv 1 writeup → [ctf-writeups/picoctf/mall.md](ctf-writeups/picoctf/mall.md)

**✅ MODUL 3 GODKÄND:** 10 PortSwigger-labbar + 30 picoCTF + writeup

---

## MODUL 4 — OSINT

**Beskrivning:**
Innan en angripare rör ett system samlar de information — öppet och passivt, utan att lämna spår. Du lär dig hur man kartlägger ett mål med bara öppen information: Google, metadata, bilder och exponerade enheter på internet.

**Förkunskapskrav:** Modul 2

**Efter denna modul kan du:**
- Hitta information om ett mål utan att kontakta det
- Använda Google Dorking för att hitta exponerade filer
- Hitta exponerade enheter och tjänster via Shodan
- Analysera bilder för att bestämma var de är tagna

---

### Teori

- [ ] Klara "Google Dorking" — hitta känslig info via Google → **tryhackme.com/room/googledorking**
- [ ] Klara "Shodan" — kartlägg exponerade enheter → **tryhackme.com/room/shodan**

### Examination
*Klara dessa på egen hand — de testar om du kan kombinera OSINT-teknikerna.*

- [ ] Klara "OhSINT" — hitta allt om en person med bara en bild → **tryhackme.com/room/ohsint**
- [ ] Klara "Searchlight - IMINT" — geolokalisera en bild → **tryhackme.com/room/searchlightosint**
- [ ] Forensics → "Trivial Flag Transfer Protocol" → **picoctf.org/practice**
- [ ] Forensics → "Enhance!" → **picoctf.org/practice**
- [ ] Forensics → "Sleuthkit Intro" → **picoctf.org/practice**

**✅ MODUL 4 GODKÄND:** OSINT + passiv spaning + 3 forensics

---

## MODUL 5 — Logganalys & Incidenthantering

**Beskrivning:**
En cybersoldat måste kunna läsa loggar och identifiera intrång. Du lär dig att följa ett angrepp steg för steg i loggdata — från första kontakt till full kompromiss — och hur man sätter upp system som automatiskt larmar vid misstänkt trafik.

**Förkunskapskrav:** Modul 2 och 3

**Efter denna modul kan du:**
- Läsa och förstå Windows- och Linux-systemloggar
- Identifiera ett pågående intrång i loggdata
- Använda Splunk för att söka och analysera loggar
- Konfigurera Snort för att detektera attacker i nätverkstrafik

---

### Teori — Loggar

- [ ] Klara "Windows Event Logs" — förstå Windows-loggar → **tryhackme.com/room/windowseventlogs**
- [ ] Klara "Linux Forensics" — förstå Linux-loggar → **tryhackme.com/room/linuxforensics**
- [ ] Klara "Splunk: Basics" — lär dig logganalysverktyget → **tryhackme.com/room/splunk101**
- [ ] Klara "Snort" — intrångsdetektering → **tryhackme.com/room/snort**

### Examination
*Klara dessa på egen hand. Du måste hitta ett riktigt angrepp i loggar.*

- [ ] Klara "Investigating with Splunk" — hitta ett angrepp i riktig loggdata → **tryhackme.com/room/investigatingwithsplunk**
- [ ] Klara "Traffic Analysis Essentials" → **tryhackme.com/room/trafficanalysisessentials**
- [ ] Klara "Incident Response and Forensics" → **tryhackme.com/room/incidentresponseintro**
- [ ] Forensics → "Operation Oni" → **picoctf.org/practice**
- [ ] Forensics → "Eavesdrop" → **picoctf.org/practice**
- [ ] Totalt 40 lösta picoCTF utmaningar → **picoctf.org/practice**

**✅ MODUL 5 GODKÄND:** Logganalys + IDS + 40 picoCTF

---

## MODUL 6 — Attacktekniker & Penetrationstestning

**Beskrivning:**
Nu kombinerar du allt du lärt dig och angriper riktiga system. Du lär dig den fullständiga pentesting-metodologin — från spaning till intrång till att bli admin — och automatiserar delar av arbetet med Python.

**Förkunskapskrav:** Modul 2, 3 och 5

**Efter denna modul kan du:**
- Genomföra ett fullständigt penetrationstest (recon → exploit → root)
- Eskalera rättigheter från vanlig användare till admin/root
- Använda Metasploit för att exploatera kända sårbarheter
- Skriva egna attack-scripts i Python

---

### Teori

- [ ] Klara "Metasploit: Introduction" — lär dig ramverket → **tryhackme.com/room/metasploitintro**
- [ ] Klara "Privilege Escalation" — lär dig bli admin → **tryhackme.com/room/privescpending**
- [ ] Klara "Hello World" till "Functions" — Python-grunder → **learnpython.org**

### Praktik

- [ ] Klara "Blue" — exploatera Windows med Metasploit → **tryhackme.com/room/blue**
- [ ] Klara "Ice" — fullständig Windows exploitation → **tryhackme.com/room/ice**

### Examination
*Klara dessa på egen hand utan walkthrough. Skriv writeup för varje.*

- [ ] Starting Point → "Meow" → **hackthebox.com/starting-point**
- [ ] Starting Point → "Fawn" → **hackthebox.com/starting-point**
- [ ] Starting Point → "Dancing" → **hackthebox.com/starting-point**
- [ ] Starting Point → "Redeemer" → **hackthebox.com/starting-point**
- [ ] Starting Point → "Explosion" → **hackthebox.com/starting-point**
- [ ] Machines → klara 5 Easy-maskiner → **hackthebox.com/machines**
- [ ] Skriv writeup för varje maskin → [ctf-writeups/hackthebox/mall.md](ctf-writeups/hackthebox/mall.md)
- [ ] Skriv ett eget port-scanning script i Python → [notes/verktyg/cheatsheet.md](notes/verktyg/cheatsheet.md)

**✅ MODUL 6 GODKÄND:** 10 HTB-maskiner + writeups + Python-script

---

## MODUL 7 — Live CTF & Avancerat

**Beskrivning:**
Sista modulen. Du tävlar nu mot riktiga människor under tidspress och visar att du kan lösa okända problem på egen hand. Du bygger också ett komplett portfolio som dokumenterar hela din resa.

**Förkunskapskrav:** Modul 1–6

**Efter denna modul kan du:**
- Lösa okända CTF-utmaningar under tidspress
- Förklara och dokumentera dina lösningar i writeups
- Genomföra Red Team-operationer
- Visa upp ett portfolio över din tekniska kompetens

---

### Teori — Avancerat

- [ ] Klara hela "Junior Penetration Tester"-pathen → **tryhackme.com/path/outline/jrpenetrationtester**
- [ ] Klara "Red Team Fundamentals" → **tryhackme.com/room/redteamfundamentals**
- [ ] Klara "Red Team Recon" → **tryhackme.com/room/redteamrecon**

### Examination — Live tävling

- [ ] Delta i picoCTF live-tävlingen (mars varje år) → **picoctf.org**
- [ ] Lös minst 10 utmaningar i live-tävlingen
- [ ] Delta i en extern CTF → **ctftime.org**
- [ ] Lös minst 5 utmaningar i extern CTF
- [ ] Nå rank "Hacker" på HackTheBox → **hackthebox.com**
- [ ] Ha minst 10 writeups uppladdade i repot → [ctf-writeups/](ctf-writeups/)

**✅ MODUL 7 GODKÄND:** Tekniskt redo för cyberoperationer

---

## Totalt framsteg
- picoCTF utmaningar: 0 / 40+
- PortSwigger labbar: 0 / 10
- TryHackMe rum: 0 / 20+
- HackTheBox maskiner: 0 / 10+
- Writeups: 0 / 10+

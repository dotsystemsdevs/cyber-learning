# Kommandon — Referens

---

## Python

```bash
# Kör ett Python-script
python filnamn.py
python "fil med mellanslag.py"

# Kör och se output direkt
python -c "print('hello')"

# Kolla vilken version du har
python --version
```

---

## Terminal (Windows CMD)

```bash
# Öppna en mapp
cd "C:\Users\diana\Desktop\cyber"

# Lista filer i mappen
dir

# Gå upp en nivå
cd ..

# Rensa terminalen
cls
```

---

## Terminal (Linux / Kali)

```bash
# Navigera
pwd                    # visa var du är
ls                     # lista filer
ls -la                 # lista alla filer inkl dolda
cd mapp/               # gå in i mapp
cd ..                  # gå tillbaka

# Filer
cat fil.txt            # visa innehåll
cp fil.txt kopia.txt   # kopiera
mv fil.txt nytt.txt    # flytta / byta namn
rm fil.txt             # ta bort fil
mkdir mapp             # skapa mapp

# Söka
grep "text" fil.txt    # sök efter text i fil
find / -name "fil.txt" # hitta en fil
```

---

## Nmap (port scanning)

```bash
nmap 192.168.1.1          # enkel skanning
nmap -sV 192.168.1.1      # visa tjänsteversioner
nmap -p 80,443 192.168.1.1 # skanna specifika portar
nmap -p- 192.168.1.1      # skanna ALLA portar
nmap -A 192.168.1.1       # aggressiv (OS, version, scripts)
```

---

## Wireshark (filter)

```
http                        # visa bara HTTP-trafik
ip.addr == 192.168.1.1     # trafik till/från en IP
tcp.port == 80              # trafik på port 80
dns                         # visa bara DNS-trafik
```

---

## Git

```bash
git status                  # se vad som ändrats
git add filnamn.md          # lägg till fil
git add -A                  # lägg till allt
git commit -m "meddelande"  # spara ändring
git push                    # ladda upp till GitHub
git pull                    # hämta senaste från GitHub
```

---

## ASCII

ASCII är en standard som kopplar siffror till tecken.
Varje bokstav, siffra och symbol har ett unikt nummer.

```python
ord('A')    # → 65   (tecken till siffra)
chr(65)     # → 'A'  (siffra till tecken)

ord('a')    # → 97
chr(97)     # → 'a'
```

| Tecken | ASCII-värde |
|--------|-------------|
| A | 65 |
| Z | 90 |
| a | 97 |
| z | 122 |
| 0 | 48 |
| 9 | 57 |
| mellanslag | 32 |

---

## Kryptografi (CryptoHack / CTF)

```python
# XOR två värden
0x32 ^ 81           # = 99

# Omvandla siffra till tecken
chr(99)             # = 'c'

# Omvandla tecken till siffra
ord('c')            # = 99

# Avkoda Base64
import base64
base64.b64decode("SGVsbG8=")   # = b'Hello'

# Avkoda Hex
bytes.fromhex("48656c6c6f")    # = b'Hello'

# XOR hela listan (som i CryptoHack Great Snakes)
ords = [81, 64, 75]
"".join(chr(o ^ 0x32) for o in ords)
```

---

## Burp Suite

```
Proxy → Intercept ON    # fånga HTTP-requests
Repeater               # skicka om requests med ändringar
Intruder               # brute force
```

---

## Python — Enkel port scanner

```python
import socket

host = "127.0.0.1"
for port in range(1, 1025):
    s = socket.socket()
    result = s.connect_ex((host, port))
    if result == 0:
        print(f"Port {port} öppen")
    s.close()
```

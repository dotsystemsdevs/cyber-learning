# Modul 1 — Introduktion till Cybersäkerhet

## CIA-triaden

| | Princip | Betyder | Bryts av | Skyddas med |
|---|---|---|---|---|
| C | Confidentiality | Bara behöriga får se datan | Phishing, sniffing | Kryptering, MFA |
| I | Integrity | Data får inte ändras obehörigt | MitM, SQL Injection | Hashing, signaturer |
| A | Availability | System måste vara tillgängliga | DDoS, Ransomware | Backuper, redundans |

---

## Etisk Hacking

Etisk hacking = auktoriserat testande av system för att hitta sårbarheter innan angripare gör det.
- Skillnaden mot oetisk hacking: etiska hackare har **tillstånd**
- Kallas också: penetrationstestning / red teaming

---

## Kryptografi

### Typer
- **Symmetrisk** — Samma nyckel för kryptering och dekryptering (AES)
- **Asymmetrisk** — Publik nyckel krypterar, privat nyckel dekrypterar (RSA)
- **Hashing** — Envägsfunktion, kan inte dekrypteras (MD5, SHA-256)

### Vanliga chiffer i CTF
| Chiffer | Hur det fungerar | Exempel |
|---------|-----------------|---------|
| Caesar | Förskjut bokstäver med X steg | A→D (steg 3) |
| Base64 | Kodar binär data som text | SGVsbG8= = "Hello" |
| ROT13 | Caesar men alltid 13 steg | A→N |
| Hex | Hexadecimalt | 48 65 6c 6c 6f = "Hello" |
| ASCII | Siffror 0–127 kopplade till tecken | 65 = 'A', 97 = 'a' |

### ASCII
ASCII är en 7-bitars standard som kopplar heltal (0–127) till tecken.
Används ofta i CTF för att dölja text som en lista med siffror.

| Tecken | ASCII |
|--------|-------|
| A | 65 |
| Z | 90 |
| a | 97 |
| z | 122 |
| 0 | 48 |
| { | 123 |
| } | 125 |

### Verktyg
- [CyberChef](https://gchq.github.io/CyberChef/) — dekryptera nästan vad som helst
- [Hashcat](https://hashcat.net/hashcat/) — cracka hash-lösenord

---

## Kommandon — Python (krypto)

```python
# Tecken → siffra
ord('A')    # = 65

# Siffra → tecken
chr(65)     # = 'A'

# Avkoda en lista med ASCII-tal till text (CTF-flagga)
nums = [99, 114, 121, 112, 116, 111, 123, 65, 83, 67, 73, 73, 95, 112, 114, 49, 110, 116, 52, 98, 108, 51, 125]
print(''.join(chr(n) for n in nums))   # = crypto{ASCII_pr1nt4bl3}

# Loopa ett tecken i taget
for n in nums:
    print(chr(n))

# Avkoda Base64
import base64
base64.b64decode("SGVsbG8=")                  # = b'Hello'

# Avkoda Hex
bytes.fromhex("48656c6c6f")                   # = b'Hello'

# Koda Hex → Base64 (två steg, inifrån och ut)
base64.b64encode(bytes.fromhex("72bca9b68fc16ac7beeb8f849dca1d8a783e8acf9679bf9269f7bf"))
# Steg 1: bytes.fromhex() → översätter hex-text till rå bytes
# Steg 2: b64encode()     → kodar bytes till Base64
# OBS: b64encode() kräver bytes, INTE en vanlig sträng

# XOR två värden
0x32 ^ 81   # = 99

# XOR hela listan
ords = [81, 64, 75]
''.join(chr(o ^ 0x32) for o in ords)
```

---

## Mina anteckningar
*(Lägg till vad du vill komma ihåg här)*

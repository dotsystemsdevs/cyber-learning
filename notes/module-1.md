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

### ASCII — tecken och siffror
```python
ord('A')        # Tecken → siffra = 65
chr(65)         # Siffra → tecken = 'A'

# Avkoda en lista med ASCII-tal till text
nums = [99, 114, 121, 112, 116, 111, 123, ...]
print(''.join(chr(n) for n in nums))   # = crypto{ASCII_pr1nt4bl3}

# Loopa ett tecken i taget
for n in nums:
    print(chr(n))
```

### Hex
```python
bytes.fromhex("48656c6c6f")   # Hex → bytes = b'Hello'
```

### Base64
```python
import base64
base64.b64decode("SGVsbG8=")  # Base64 → bytes = b'Hello'
base64.b64encode(b"Hello")    # bytes → Base64 = b'SGVsbG8='

# Hex → Base64 (gå via bytes, aldrig direkt från sträng)
base64.b64encode(bytes.fromhex("72bca9b68fc16ac7beeb8f849dca1d8a783e8acf9679bf9269f7bf"))
```

### Big Integers (PyCryptodome)
```python
from Crypto.Util.number import long_to_bytes, bytes_to_long

long_to_bytes(11515195063862318899931685488813747395775516287289682636499965282714637259206269)
# = b'crypto{3nc0d1n6_4ll_7h3_w4y_d0wn}'

bytes_to_long(b"Hello")   # bytes → stort heltal
```

### XOR
```python
108 ^ 13        # XOR två värden = 97

# XOR hela listan
ords = [81, 64, 75]
''.join(chr(o ^ 0x32) for o in ords)
```

---

## Mina anteckningar
*(Lägg till vad du vill komma ihåg här)*

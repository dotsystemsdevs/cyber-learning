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

### XOR
XOR jämför två tal bit för bit — samma bitar ger 0, olika ger 1.

```
  01101100   (108 = 'l')
^ 00001101   (13)
-----------
  01100001   (97 = 'a')
```

| Egenskap | Formel | Betyder |
|----------|--------|---------|
| Commutative | A ⊕ B = B ⊕ A | Ordningen spelar ingen roll |
| Associative | A ⊕ (B ⊕ C) = (A ⊕ B) ⊕ C | Parenteser spelar ingen roll |
| Identity | A ⊕ 0 = A | XOR med 0 ändrar ingenting |
| Self-Inverse | A ⊕ A = 0 | Något XOR med sig självt = 0 |

Self-Inverse är viktig i krypto: om `flagga ⊕ nyckel = krypterad`, då är `krypterad ⊕ nyckel = flagga`.

### Verktyg
- [CyberChef](https://gchq.github.io/CyberChef/) — dekryptera nästan vad som helst
- [Hashcat](https://hashcat.net/hashcat/) — cracka hash-lösenord

---

## Kommandon — Python (krypto)

### ASCII
```python
ord('A')                          # Tecken → siffra = 65
chr(65)                           # Siffra → tecken = 'A'
''.join(chr(n) for n in nums)     # Lista → text
```

### Hex
```python
bytes.fromhex("48656c6c6f")       # Hex → bytes = b'Hello'
```

### Base64
```python
import base64
base64.b64decode("SGVsbG8=")      # Base64 → bytes = b'Hello'
base64.b64encode(b"Hello")        # bytes → Base64 = b'SGVsbG8='
base64.b64encode(bytes.fromhex("72bca9..."))  # Hex → Base64
```

### Big Integers
```python
from Crypto.Util.number import long_to_bytes, bytes_to_long
long_to_bytes(11515195063862318899931685488813747395775516287289682636499965282714637259206269)
bytes_to_long(b"Hello")           # bytes → stort heltal
```

### XOR
```python
108 ^ 13                          # XOR två värden = 97
''.join(chr(o ^ 0x32) for o in ords)  # XOR hela listan
```

---

## Mina anteckningar
*(Lägg till vad du vill komma ihåg här)*

# Modul 2 — Linux & Nätverk

## Linux

### Navigation
| Kommando | Vad det gör |
|----------|-------------|
| `pwd` | Visa var du är |
| `ls` | Lista filer |
| `ls -la` | Lista alla filer inkl dolda |
| `cd mapp` | Gå in i mapp |
| `cd ..` | Gå tillbaka |

### Filer
| Kommando | Vad det gör |
|----------|-------------|
| `cat fil.txt` | Visa innehåll |
| `cp fil.txt kopia.txt` | Kopiera fil |
| `mv fil.txt ny.txt` | Flytta/byta namn |
| `rm fil.txt` | Ta bort fil |
| `mkdir mapp` | Skapa mapp |

### Sökning
| Kommando | Vad det gör |
|----------|-------------|
| `grep "text" fil.txt` | Sök efter text i fil |
| `find / -name "fil.txt"` | Hitta fil |

---

## Nätverk

### OSI-modellen
| Lager | Namn | Exempel |
|-------|------|---------|
| 7 | Applikation | HTTP, DNS, FTP |
| 6 | Presentation | SSL/TLS, kryptering |
| 5 | Session | Uppkopplingar |
| 4 | Transport | TCP, UDP |
| 3 | Nätverk | IP-adresser |
| 2 | Datalänk | MAC-adresser |
| 1 | Fysisk | Kablar, wifi |

### Viktiga portar
| Port | Protokoll | Syfte |
|------|-----------|-------|
| 21 | FTP | Filöverföring |
| 22 | SSH | Säker terminal |
| 23 | Telnet | Terminal (osäker) |
| 80 | HTTP | Webb |
| 443 | HTTPS | Säker webb |
| 3306 | MySQL | Databas |

### TCP vs UDP
- **TCP** — Säker, kontrollerar att paket kommer fram (webb, email)
- **UDP** — Snabb, kontrollerar inte (video, gaming)

---

## Kommandon — Linux & Nätverk

```bash
# Visa IP-adress
ifconfig

# Testa anslutning
ping google.com

# nmap — port scanning
nmap 192.168.1.1             # Enkel skanning
nmap -sV 192.168.1.1         # Visa versioner på tjänster
nmap -p 80,443 192.168.1.1   # Skanna specifika portar
nmap -p- 192.168.1.1         # Skanna ALLA portar
nmap -A 192.168.1.1          # Aggressiv skanning (OS, version, scripts)
```

### Wireshark filter
```
http                          # Visa bara HTTP-trafik
ip.addr == 192.168.1.1        # Trafik till/från IP
tcp.port == 80                # Trafik på port 80
```

---

## Mina anteckningar
*(Lägg till vad du vill komma ihåg här)*

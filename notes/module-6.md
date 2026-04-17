# Modul 6 — Attacktekniker & Penetrationstestning

## Malware

### Typer
| Typ | Vad det gör |
|-----|-------------|
| Virus | Infekterar filer, sprider sig |
| Mask (Worm) | Sprider sig via nätverk utan hjälp |
| Trojan | Ser ut som legitim mjukvara |
| Ransomware | Krypterar dina filer, kräver lösen |
| Spyware | Spionerar på användaren |
| Rootkit | Gömmer sig djupt i systemet |
| Keylogger | Spelar in tangenttryckningar |

### Hur malware sprids
- Phishing-mejl med bifogad fil
- Infekterade USB-minnen
- Drive-by downloads (besöka infekterad webbsida)
- Sårbar mjukvara som inte är uppdaterad

### Analys
- **Statisk analys** — Titta på koden utan att köra den
- **Dynamisk analys** — Kör malware i en sandbox och observera beteendet

### Verktyg
- VirusTotal (online) — ladda upp fil för analys
- Any.run (online sandbox)
- Ghidra — reverse engineering

---

## Metasploit
*(Fyll i här när du klarar Metasploit-modulen)*

## Privilege Escalation
*(Fyll i här)*

## HackTheBox — maskiner
*(Fyll i maskin för maskin här)*

---

## Kommandon — Python scripting

```python
import socket

# Enkel port scanner
host = "127.0.0.1"
for port in range(1, 1025):
    s = socket.socket()
    result = s.connect_ex((host, port))
    if result == 0:
        print(f"Port {port} öppen")
    s.close()
```

---

## Mina anteckningar
*(Lägg till vad du vill komma ihåg här)*

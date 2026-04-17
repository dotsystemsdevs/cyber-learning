# Verktyg — Cheatsheet

## nmap (port scanning)
```bash
nmap 192.168.1.1          # Enkel skanning
nmap -sV 192.168.1.1      # Visa versioner på tjänster
nmap -p 80,443 ip         # Skanna specifika portar
nmap -p- ip               # Skanna ALLA portar
nmap -A ip                # Aggressiv skanning (OS, version, scripts)
```

## Wireshark (nätverksanalys)
- Öppna Wireshark → välj nätverkskort → klicka Start
- Filter: `http` — visa bara HTTP-trafik
- Filter: `ip.addr == 192.168.1.1` — visa trafik till/från IP
- Filter: `tcp.port == 80` — visa trafik på port 80

## Burp Suite (webb)
- Proxy → Intercept ON → Fånga HTTP-requests
- Repeater → Skicka om requests med ändringar
- Intruder → Brute force

## Python (scripting)
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

## Anteckningar
*(Skriv dina egna anteckningar här)*

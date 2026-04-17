# Modul 3 — Webbattacker

## SQL Injection
Angriparen skriver SQL-kod i ett formulär för att manipulera databasen.

**Exempel:**
```
username: admin' OR '1'='1
```
→ Loggar in utan lösenord

**Testa med:** PortSwigger SQL Injection labs

## XSS (Cross-Site Scripting)
Angriparen injicerar JavaScript i en webbsida som körs i andras webbläsare.

**Exempel:**
```html
<script>alert('XSS')</script>
```

**Testa med:** PortSwigger XSS labs

## CSRF (Cross-Site Request Forgery)
Lurar en inloggad användare att utföra oönskade handlingar.

## Brute Force
Testa alla möjliga lösenord tills rätt hittas.
**Verktyg:** Hydra, Burp Suite Intruder

## OWASP Top 10
| # | Sårbarhet |
|---|-----------|
| 1 | Broken Access Control |
| 2 | Cryptographic Failures |
| 3 | Injection (SQL, XSS) |
| 4 | Insecure Design |
| 5 | Security Misconfiguration |
| 6 | Vulnerable Components |
| 7 | Authentication Failures |
| 8 | Integrity Failures |
| 9 | Logging Failures |
| 10 | Server-Side Request Forgery |

---

## Kommandon — Burp Suite

```
Proxy → Intercept ON    # Fånga HTTP-requests
Repeater               # Skicka om requests med ändringar
Intruder               # Brute force
```

---

## Mina anteckningar
*(Lägg till vad du vill komma ihåg här)*

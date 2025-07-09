# Vunerabillity-Assesment-jucie-shop
 
🔐 Web Application Penetration Testing – OWASP Juice Shop
🎯 Project Overview
This repository documents a full-scale penetration test on OWASP Juice Shop, a deliberately insecure web application used to learn about modern web vulnerabilities. The assessment was conducted using the OWASP Top 10 framework, with a combination of automated tools and manual techniques.

🧰 Tools & Technologies
Reconnaissance: Nmap, Subfinder, AMASS, FFUF, HTTPX, theHarvester

Scanning & Exploitation: Burp Suite, OWASP ZAP

Manual Testing: Parameter tampering, JWT abuse, session hijacking, SQLi payloads

🚨 Discovered Vulnerabilities
No	Vulnerability	Description / Impact
1	Broken Access Control	Cart manipulation via BasketId override
2	SQL Injection	Login bypass, DB manipulation
3	Cross-Site Scripting (XSS)	Session theft, DOM/UI manipulation
4	CSRF	Forced user actions via crafted HTML
5	Null Byte Injection	Bypass filters to access sensitive .md backups
6	SSTI	Remote code execution via injected payloads
7	Password Reset Exploit	Unauthorized reset by removing currentPassword
8	XXE	File disclosure using malicious XML (/etc/passwd)

🔒 Remediation Recommendations
✅ Input validation and output encoding

✅ Parameterized queries (avoid raw SQL)

✅ CSRF protection tokens + origin validation

✅ Disable public admin role creation

✅ Secure session management (e.g., JWT hardening)

✅ Enable CSP headers, sanitize user input

✅ Regular patching & CVE monitoring

✅ Security awareness for developers

📊 Outcome
This project demonstrates how real-world web vulnerabilities can be discovered, exploited, and documented ethically. The goal is to raise awareness of secure coding practices and encourage better web security implementation.
 
🤝 Disclaimer
This project was conducted in a controlled environment using OWASP Juice Shop, a legal, intentionally vulnerable app for cybersecurity education.
Do not attempt these techniques on unauthorized systems.

You can view the full report hosted on Notion here: https://concise-hurricane-b7d.notion.site/22bb5694af9d801790b9cba4202ee144?pvs=141

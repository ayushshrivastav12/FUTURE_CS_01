# DVWA Security Testing Report

## 🔍 Objective
Perform manual security testing on DVWA to identify:
- SQL Injection
- Cross-Site Scripting (XSS)
- Authentication Flaws

## 🧰 Tools Used
- Docker
- DVWA (Damn Vulnerable Web App)
- Browser (manual testing)

## ✅ Vulnerabilities Identified

### 1. SQL Injection
- Payloads: `1' OR 1=1 --`, `-1' UNION SELECT null, database() --`
- Triggered SQL errors & data leaks
- Screenshots: `sqli.png`, `sqli_fatal_error.png`

### 2. Cross-Site Scripting (XSS)
- Payload: `<script>alert('Hacked by Ayush')</script>`
- Reflected XSS confirmed via alert box

### 3. Authentication Flaw
- Weak default credentials (`admin/password`) accepted
- No brute-force protection or 2FA

## 📎 Report
See `Security_Testing_Report.docx` for full documentation.

---

**Prepared by:** Ayush Shrivastav  
**Date:** July 10, 2025

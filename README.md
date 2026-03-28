# 🔐 API Security Risk Analysis Report



## 📌 Project Overview

This project presents a hands-on API Security Risk Assessment conducted on two public demo APIs — **JSONPlaceholder** and **ReqRes** — following the **OWASP API Security Top 10 (2023)** framework. All testing was performed using Postman and Browser DevTools.

The goal was to identify real-world API vulnerabilities, classify their severity, assess business impact, and provide actionable remediation guidance — documented in a professional security report.

 **Built as part of my Future Interns Cybersecurity Internship - Task 3**
 
---

## 🎯 APIs Tested

| API | Base URL | Purpose |
|-----|----------|---------|
| JSONPlaceholder | https://jsonplaceholder.typicode.com | Fake REST API for testing |
| ReqRes | https://reqres.in | API testing & prototyping platform |

---

## 🛠️ Tools Used

- **Postman** — endpoint testing & request crafting
- **Browser DevTools** — response header inspection
- **OWASP API Security Top 10** — risk classification framework

---

## 🚨 Findings Summary

| # | Risk | Severity | OWASP Category |
|---|------|----------|----------------|
| 1 | No Authentication on Any Endpoint | 🔴 Critical | API2 – Broken Authentication |
| 2 | Unrestricted HTTP Methods (PUT/DELETE) | 🔴 Critical | API5 – Broken Function Level Auth |
| 3 | No Rate Limiting | 🟠 High | API4 – Unrestricted Resource Consumption |
| 4 | Sensitive Data Exposure in Responses | 🟠 High | API3 – Broken Object Property Level Auth |
| 5 | Missing Security Headers | 🟡 Medium | API8 – Security Misconfiguration |
| 6 | Excessive Data Exposure | 🟡 Medium | API3 – Broken Object Property Level Auth |
| 7 | Predictable Sequential Resource IDs | 🟢 Low | API1 – Broken Object Level Auth |
| 8 | No HTTPS Enforcement / Missing HSTS | ℹ️ Info | API8 – Security Misconfiguration |

---

## 📸 Screenshots

### 1. No Authentication — GET /users returns full PII with 200 OK
<img width="1216" height="790" alt="Screenshot 2026-03-28 131017" src="https://github.com/user-attachments/assets/962ea224-e0f3-4e59-b39e-cbcecacffb03" />


### 2. Unauthenticated DELETE — post deleted with no credentials
<img width="1192" height="798" alt="Screenshot 2026-03-28 131126" src="https://github.com/user-attachments/assets/69cc2d2a-983f-44d5-bb56-05b78c78465e" />


### 3. Excessive Data Exposure — email, address, geo coordinates returned anonymously
<img width="1226" height="850" alt="Screenshot 2026-03-28 131736" src="https://github.com/user-attachments/assets/d388d59f-e7a6-4d1b-b122-7c17db02a726" />


### 4. Missing Security Headers — no CSP, HSTS, or X-Frame-Options in response
<img width="1919" height="924" alt="Screenshot 2026-03-28 132154" src="https://github.com/user-attachments/assets/cc1157d0-ac0d-4c1c-83b9-8303efd7be77" />


### 5. Unauthorized PUT — data modified with no token, 200 OK returned
<img width="1211" height="852" alt="Screenshot 2026-03-28 131432" src="https://github.com/user-attachments/assets/c3d6e409-cc4b-461d-9858-a392e400d2ec" />


---



## 📚 References

- [OWASP API Security Top 10](https://github.com/OWASP/API-Security)
- [JSONPlaceholder](https://jsonplaceholder.typicode.com)
- [ReqRes](https://reqres.in)

---
## 👤 Author
Asna Haris — Cybersecurity Intern

GitHub: https://github.com/asnahar1s

LinkedIn: https://www.linkedin.com/in/asna-haris-684058319

## 📄 License
This project is built as part of my Cybersecurity Internship Program.

Website: https://www.futureinterns.com/





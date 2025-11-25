# 1️⃣ Introduction

**Tester(s):**  
- Name:  Suvi Perkiö

**Purpose:**  
- Sivustolle rekisteröitäessä turvallisuus riskien löytäminen

**Scope:**  
- Tested components:  Rekisteröityminen ja autentikaatio
- Exclusions:  
- Test approach: Gray-box

**Test environment & dates:**  
- Start:  22.11.22025
- End:  25.11.2025
- Test environment details (OS, runtime, DB, browsers): Docker, ZAP, Powershell

**Assumptions & constraints:**  
- Rajoitettu aika, sovellusten konfiguraatio

---

# 2️⃣ Executive Summary

**Short summary (1-2 sentences):**  

**Overall risk level:** (Low / Medium / High / Critical)

**Top 5 immediate actions:**  
1. Path traversal. High. Input validation (tarkistaa inputin arvon ja poistaa turhat/vaaralliset merkit, inputin pituuden jne.). Ja turvallinen kansioiden hallinta.
2. SQL injection. High. Käyttää vain parametrisoituja tietokantakyselyitä(SQL quer).
3. Format string error. Medium. String input validation(validoi string inputin muoto, kieltämällä väärät merkit stringistä).
4. Content Security Policy header not set. Medium. Konfiguroida ja aktivoida CSP header.
5. Missing Anti-clickjacking header. Medium. Lisää ja aktivoi CSP header.

---

# 3️⃣ Severity scale & definitions

|  **Severity Level**  | **Description**                                                                                                              | **Recommended Action**           |
| -------------------- | ---------------------------------------------------------------------------------------------------------------------------- | -------------------------------- |
|      🔴 **High**     | A serious vulnerability that can lead to full system compromise or data breach (e.g., SQL Injection, Remote Code Execution). | *Immediate fix required*         |
|     🟠 **Medium**    | A significant issue that may require specific conditions or user interaction (e.g., XSS, CSRF).                              | *Fix ASAP*                       |
|      🟡 **Low**      | A minor issue or configuration weakness (e.g., server version disclosure).                                                   | *Fix soon*                       |
| 🔵 **Info** | No direct risk, but useful for system hardening (e.g., missing security headers).                                            | *Monitor and fix in maintenance* |


---

# 4️⃣ Findings (filled with examples → replace)

> Fill in one row per finding. Focus on clarity and the most important issues.

| ID | Severity | Finding | Description | Evidence / Proof |
|------|-----------|----------|--------------|------------------|
| F-01 | 🔴 High | SQL Injection in registration | Input field allows `' OR '1'='1` injection | Screenshot or sqlmap result |
| F-02 | 🟠 Medium | Session fixation | Session ID remains unchanged after login | Burp log or response headers |
| F-03 | 🟡 Low | Weak password policy | Accepts passwords like "12345" | Screenshot of registration success |

---

> [!NOTE]
> Include up to 5 findings total.   
> Keep each description short and clear.

---

# 5️⃣ OWASP ZAP Test Report (Attachment)

**Purpose:**  
- Attach or link your OWASP ZAP scan results (Markdown format preferred).

---

**Instructions (CMD version):**
1. Run OWASP ZAP baseline scan:  
   ```bash
   zap-baseline.py -t https://example.com -r zap_report_round1.html -J zap_report.json
   ```
2. Export results to markdown:  
   ```bash
   zap-cli report -o zap_report_round1.md -f markdown
   ```
3. Save the report as `zap_report_round1.md` and link it below.

---
> [!NOTE]
> 📁 **Attach full report:** → `check itslearning` → **Add a link here**

---

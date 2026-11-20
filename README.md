# Week 03 — Password Security Audit & Hash Analysis

**Internship:** Networkwalks Academy — Cybersecurity Internship
**Track:** Digital Safety Associate | SOC Analyst Fundamentals
**Focus:** Password Strength Auditing, Hash Analysis, Defensive Controls

---

## Overview

In Week 03, I audited password-protected PDF files provided in an authorized lab environment to evaluate how weak passwords create risk for organizations.

The goal was not just to unlock files, but to understand from a SOC Analyst perspective:
Why do weak passwords fail, and how should organizations defend against them?

Two different auditing approaches were tested and cross-verified:
1.  **W3-PM1:** Offline audit using Johnny (John the Ripper GUI)
2.  **W3-PM2:** Browser-based audit using Networkwalks Hash & Password Auditing Tools

## Scope & Ethics

> All testing was performed only on lab-provided files in an authorized training environment.
> No real-world systems, personal accounts, or unauthorized targets were tested.

## Lab Environment

- **OS:** Windows 11
- **Audit Tools:** Johnny (JTR GUI), Networkwalks Auditing Tools
- **Target Type:** Password-protected PDF files (Lab Provided)

## Methodology — High Level

**1. W3-PM1 — Offline Audit**
- Analyzed the protection applied to the lab PDF files.
- Performed an authorized dictionary audit to test password strength.
- Verified access after recovery and documented the result.

**2. W3-PM2 — Online Audit & Verification**
- Re-audited the same lab files using browser-based tools.
- Cross-checked results from PM1 to confirm consistency.
- Captured the lab flag as proof of successful verification.

## Results Summary

| Task | Tool Used | Status |
| :--- | :--- | :--- |
| W3-PM1 | Johnny (JTR GUI) | ✅ Completed |
| W3-PM2 | Networkwalks Tools | ✅ Completed |
| Verification | Flags Captured | ✅ Verified |

*Detailed passwords and flags are intentionally not published for security best practice.*

## Proof of Execution

### PM1 — Johnny Audit Result
![Johnny Result](./W3-PM1-Password-Cracking-JTR/PM1-Johnny-Result.png)

### PM2 — Networkwalks Audit Result
![NW Tools Result](./W3-PM2-Password-Cracking-NW-Tools/PM2-NW-Tools-Result.png)

### Lab Flag — Captured
![Flag](./W3-PM2-Password-Cracking-NW-Tools/Flag-Captured.png)

## Key Learnings for SOC

1.  **Predictable Patterns Fail Fast:** Dictionary words and keyboard patterns are recovered within minutes. They should never be used for sensitive documents.
2.  **Password Policy Matters:** 14+ character passphrases with mixed characters, plus MFA, drastically reduce this risk.
3.  **Defense-in-Depth:** SOC teams should monitor for weak credential policies, enforce password managers, and alert on repeated failed access attempts.

---
**Author:** Ahmad Raza — Ghallu305
**Week:** 03 / Networkwalks Academy

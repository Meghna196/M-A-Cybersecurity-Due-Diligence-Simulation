# NovaPay M&A Cybersecurity Due Diligence Simulation

This project simulates a pre-acquisition cybersecurity review of a fictional fintech company.
Deliverables include a NIST CSF 2.0 / CIS Controls v8 framework assessment, a risk register
with likelihood-impact scoring, a remediation roadmap organized by time horizon, and an
executive summary report written for a non-technical board audience.

**Frameworks used:** NIST CSF 2.0, CIS Controls v8, NIST SP 800-61
**Tools used:** Excel (openpyxl), PDF reporting

---

## Scenario

Meridian Financial Group is acquiring **NovaPay Technologies**, a fintech startup that processes
payments for 200,000 small businesses, in an **$85M** deal. The security team was given four weeks
to assess NovaPay's posture before board sign-off, working from a vendor questionnaire, a partial
network diagram, and a technology inventory. *(All companies and data are fictional.)*

## Headline Result

**Overall acquisition risk rating: HIGH** — 2 Critical, 3 High, and 3 Medium risks, concentrated in
identity management, endpoint security, and incident-response readiness. All are remediable; the two
Critical items are recommended as pre-close conditions.

## Deliverables

| File | What it contains |
|------|------------------|
| `01-scenario-brief.pdf` | Business context, deal facts, and NovaPay's technology stack |
| `02-framework-assessment.xlsx` | Three tabs: **Framework Mapping** (22 NIST CSF x CIS questions with maturity scores), **Findings Log** (8 findings), **Risk Register** (8 risks with live likelihood x impact formulas) |
| `03-remediation-roadmap.pdf` | Phased plan (pre-close / 30-90 / 90-180 days) mapped to People, Process, Technology |
| `04-executive-summary-report.pdf` | Six-section board report translating technical findings into business risk |
| `scenario-brief.md` | Editable source for the scenario brief |

## Risk Scoring Model

- **Risk Score = Likelihood (1-5) × Impact (1-5)**
- Bands: 1-8 Low · 9-14 Medium · 15-19 High · 20-25 Critical
- Maturity scale: 1 Not implemented · 2 Partial/informal · 3 Defined · 4 Managed/measured · 5 Optimized

## Top Findings

1. **F-001 — Incomplete MFA (Critical):** Okta covers only 60% of staff; payment access reachable without MFA.
2. **F-002 — No EDR (Critical):** Windows 10 endpoints unmonitored; usable as a pivot into the payment environment.
3. **F-003 — Legacy Oracle DB outside cloud security scope (High):** 3 years of transaction data in a monitoring blind spot.
4. **F-005 — No incident response plan (High):** PCI 12.10 and state breach-notification timelines at risk.
5. **F-006 — No vulnerability management program (High):** Known CVEs could persist unpatched in a payment platform.

## Skills Demonstrated

- Applied NIST CSF 2.0 and CIS Controls v8 across all six framework functions
- Built a formal risk register using likelihood-impact scoring with business-language risk statements
- Authored an executive due-diligence report for a non-technical board audience
- Produced a phased remediation roadmap mapped to people / process / technology
- Mapped regulatory implications across PCI DSS and SOC 2

*Relevant roles: GRC Analyst, Security Consultant, Third-Party Risk Analyst, M&A Security Advisor, Cybersecurity Due Diligence Specialist.*

# M&A Cybersecurity Due Diligence Simulation

> A structured simulation of the cybersecurity due diligence process for a fictional acquisition target, producing a risk register, gap analysis, and executive briefing aligned to NIST CSF and CIS Controls.

## Overview

Mergers and acquisitions introduce significant cybersecurity risk. Acquiring organizations inherit the target's vulnerabilities, compliance gaps, technical debt, and potential regulatory exposure. Security teams are increasingly expected to contribute formal assessments before a deal closes, yet few portfolios demonstrate this capability directly.

This project simulates the full due diligence lifecycle for a fictional mid-size SaaS company ("AcquiCo") being evaluated for acquisition. I scoped the engagement, gathered simulated evidence, mapped findings to established frameworks, quantified risk, and delivered outputs that mirror what a security or GRC team would hand to deal leadership.

The goal is to demonstrate that I can translate raw technical and policy findings into structured, business-relevant risk intelligence. This matters for roles in security advisory, GRC, M&A security consulting, and enterprise risk management.

## What I Built / Key Features

- **Acquisition Target Profile:** A realistic fictional company profile including technology stack, headcount, compliance posture, and incident history used as the evidence base for the assessment.
- **Framework-Mapped Gap Analysis:** A side-by-side assessment of AcquiCo's controls against the NIST Cybersecurity Framework (CSF) five functions and selected CIS Controls v8 safeguards, with maturity ratings per domain.
- **Risk Register:** A structured register documenting identified risks with likelihood and impact scores, risk owners, remediation timelines, and deal-relevance flags indicating which findings could affect valuation or close conditions.
- **Executive Briefing Deck:** A concise slide-format report (exported to PDF) summarizing the top risks, recommended close conditions, and a proposed 90-day post-acquisition remediation roadmap.
- **Findings Traceability Matrix:** A mapping document linking each finding back to its evidence source, framework control reference, and register entry to support auditability.

## Skills & Tools Demonstrated

**Frameworks and Standards**
- NIST Cybersecurity Framework (CSF) 2.0, Identify through Recover functions
- CIS Controls v8, Implementation Groups 1 and 2
- Basic familiarity with SOC 2 Type II report review and NIST SP 800-30 risk scoring guidance

**Documentation and Reporting**
- Microsoft Excel / Google Sheets for risk register construction and scoring models
- Markdown for structured findings documentation
- LibreOffice Impress / Google Slides for executive briefing output
- PDF export for deliverable packaging

**Security Practices**
- Risk-based prioritization and likelihood-impact matrix scoring
- Control gap analysis and maturity rating
- Remediation roadmap development with ownership assignment
- Due diligence scoping and evidence request list (ERL) construction

## Architecture & Approach

The project follows a phased due diligence model that mirrors real engagement workflows. Each phase produces a discrete artifact that feeds the next.

```text
Phase 1: Scoping
  Target profile + Evidence Request List (ERL)
        |
Phase 2: Discovery
  Policy review + Technical inventory + Incident history
        |
Phase 3: Gap Analysis
  NIST CSF mapping + CIS Controls maturity rating
        |
Phase 4: Risk Register
  Scored findings + Deal-relevance flags + Owner assignment
        |
Phase 5: Reporting
  Executive briefing + Traceability matrix + Remediation roadmap
```

Key design decisions: I used NIST SP 800-30 likelihood and impact criteria rather than a proprietary model so the scoring rationale is transparent and reproducible. I separated the technical findings layer from the business risk layer deliberately, so the register can be consumed by both security engineers and deal counsel. The executive briefing is intentionally non-technical, capped at ten slides, and anchored to business outcomes rather than control identifiers.

## Suggested Repository Structure

```text
ma-due-diligence-sim/
├── README.md
├── 01-scoping/
│   ├── target-profile.md
│   └── evidence-request-list.md
├── 02-discovery/
│   ├── policy-review-notes.md
│   ├── technical-inventory.md
│   └── incident-history-summary.md
├── 03-gap-analysis/
│   ├── nist-csf-mapping.xlsx
│   └── cis-controls-maturity.xlsx
├── 04-risk-register/
│   └── risk-register.xlsx
├── 05-reporting/
│   ├── executive-briefing.pdf
│   └── findings-traceability-matrix.xlsx
└── templates/
    ├── evidence-request-list-template.md
    └── risk-register-template.xlsx
```

## What This Demonstrates to Employers

- **Shows ability to apply NIST CSF and CIS Controls** in a practical, scoped assessment rather than as an academic exercise.
- **Demonstrates familiarity with GRC workflows**, including evidence collection, control testing, and risk scoring using recognized methodology.
- **Shows ability to communicate risk to non-technical audiences**, producing executive-ready deliverables that connect security findings to deal and business outcomes.
- **Demonstrates structured thinking across a full engagement lifecycle**, from scoping and evidence requests through reporting and remediation planning.
- **Shows awareness of M&A-specific risk considerations**, including inherited liability, regulatory exposure, and close conditions, that are directly relevant to security advisory and enterprise risk roles.
- **Demonstrates documentation discipline**, with a traceability matrix linking every finding to its evidence source and framework reference, supporting auditability and peer review.

## Getting Started

**Prerequisites:** A spreadsheet application (Excel, Google Sheets, or LibreOffice Calc) and a Markdown viewer or standard text editor.

```bash
# Clone the repository
git clone https://github.com/your-username/ma-due-diligence-sim.git
cd ma-due-diligence-sim

# Review the scoping artifacts first
cat 01-scoping/target-profile.md
cat 01-scoping/evidence-request-list.md
```

Open `03-gap-analysis/nist-csf-mapping.xlsx` and `04-risk-register/risk-register.xlsx` in your spreadsheet application to review the scoring models. The `05-reporting/executive-briefing.pdf` is the final deliverable and the recommended starting point for a quick overview of outcomes.

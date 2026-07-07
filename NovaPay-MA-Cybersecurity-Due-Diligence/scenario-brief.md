# Scenario Brief — NovaPay Technologies Acquisition

**Project:** Pre-Acquisition Cybersecurity Due Diligence Review
**Acquirer:** Meridian Financial Group
**Target:** NovaPay Technologies
**Deal value:** $85,000,000
**Assessment window:** 4 weeks
**Frameworks:** NIST CSF 2.0, CIS Controls v8, NIST SP 800-61

> This is a fictional scenario created for a portfolio project. All companies, findings, and data are invented for training and demonstration purposes.

## The Situation

Meridian Financial Group is acquiring NovaPay Technologies, a fintech startup that processes payments for 200,000 small businesses. The deal is valued at $85 million. Meridian's security team has been given four weeks to assess NovaPay's security posture before the board signs off.

For the review, the team has been handed three inputs: a completed vendor security questionnaire, a partial network diagram, and a list of the technologies NovaPay runs. The job is to identify the risks, score them, and give the executive team a clear, business-language picture of what they are buying.

Because $85 million and the payment data of 200,000 businesses are on the line, every technical finding in this review is tied back to a business consequence: regulatory exposure, breach liability, deal risk, or reputational damage to Meridian post-acquisition.

## NovaPay's Technology Stack (fictional but realistic)

- **Cloud infrastructure:** AWS-hosted (EC2, S3, RDS)
- **Container platform:** Kubernetes cluster running payment microservices
- **Source control:** GitHub, a mix of public and private repositories
- **Identity / SSO:** Okta, but deployed to only 60% of staff
- **Endpoints:** Windows 10, no EDR (endpoint detection and response) deployed
- **Legacy data store:** On-prem Oracle database holding 3 years of transaction history
- **Security staffing:** No dedicated security team; a single IT admin handles "security"
- **Attestations:** SOC 2 Type I report from 18 months ago; no Type II
- **Compliance:** PCI-DSS self-assessment questionnaire (SAQ) completed, not independently audited

## Why This Matters

NovaPay is a payment processor, which places it squarely in scope for PCI DSS and makes cardholder data its most sensitive asset. The combination of a thin security function, incomplete identity controls, unmonitored endpoints, a legacy off-cloud data store, and point-in-time-only assurance means the acquisition carries material, quantifiable cybersecurity risk that the board needs to understand before close.

Every finding in this assessment traces back to one of the facts above.

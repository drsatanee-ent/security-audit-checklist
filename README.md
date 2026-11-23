# Security Audit Checklist & Risk Assessment

A practical, documentation-based portfolio project demonstrating a structured approach to reviewing application and infrastructure security controls.

> **Project type:** Security assessment documentation / portfolio  
> **Framework reference:** OWASP Top 10 (2021), OWASP Application Security Verification Standard (ASVS), and general security best practices  
> **Status:** Portfolio template — adapt and validate for each target environment

## Project objectives

- Organize security review activities into clear, repeatable control areas.
- Identify common application, API, server, and database security risks.
- Record findings with evidence, likelihood, impact, and remediation actions.
- Communicate results through a concise audit report.

## Scope

This repository provides checklists and templates for an authorized, non-destructive security review. It does not perform automated scanning, penetration testing, or certify that a system is secure. Testing must be explicitly authorized and conducted within an agreed scope.

## Repository contents

| File | Description |
|---|---|
| [Security Audit Checklist](SECURITY-AUDIT-CHECKLIST.md) | Review questions and evidence prompts |
| [OWASP Top 10](OWASP-TOP-10.md) | Risk areas to consider during application review |
| [Risk Assessment](RISK-ASSESSMENT.md) | Likelihood/impact scoring and risk register |
| [Audit Report Template](AUDIT-REPORT-TEMPLATE.md) | Reusable report structure |

## Review domains

1. Governance, scope, and asset inventory
2. Identity, authentication, and access control
3. Input validation and application security
4. API security
5. Data protection and cryptography
6. Server, network, and database security
7. Logging, monitoring, backup, and incident response
8. Secure development and vulnerability management

## Suggested workflow

1. Define authorization, scope, exclusions, and assessment dates.
2. Understand the system architecture and data classification.
3. Review each applicable control and collect evidence.
4. Record gaps and assign likelihood and impact ratings.
5. Prioritize remediation based on risk.
6. Prepare the report and agree on follow-up actions.

## Risk rating

Use the matrix in [RISK-ASSESSMENT.md](RISK-ASSESSMENT.md). Ratings in a completed assessment should be based on evidence and documented assumptions, not guesses.

## How to use

- Copy the checklist and mark each control **Pass**, **Fail**, **Needs Review**, or **Not Applicable**.
- Add evidence references without including passwords, tokens, personal data, or confidential production information.
- Create one risk-register entry for each finding.
- Tailor the report template to the authorized assessment.

## Limitations and responsible use

This is an educational portfolio artifact. A completed checklist alone does not prove the absence of vulnerabilities. Do not test systems you do not own or have explicit written permission to assess. Avoid destructive testing and protect all collected evidence.

## Author

**Portfolio:** drsatanee-ent  
**Repository:** https://github.com/drsatanee-ent/security-audit-checklist

# OWASP Top 10 — 2021 Reference

This page summarizes the OWASP Top 10:2021 web application security risk categories as prompts for a security review. It is a reference list, not a test result or certification.

| ID | Category | Review focus |
|---|---|---|
| A01:2021 | Broken Access Control | Authorization checks, least privilege, object-level access, privilege escalation |
| A02:2021 | Cryptographic Failures | Sensitive-data handling, encryption in transit/at rest, key management |
| A03:2021 | Injection | Parameterized queries, safe command construction, input handling |
| A04:2021 | Insecure Design | Threat modeling, secure design requirements, abuse cases |
| A05:2021 | Security Misconfiguration | Secure defaults, unnecessary features, headers, cloud and server configuration |
| A06:2021 | Vulnerable and Outdated Components | Dependency inventory, patching, known-vulnerability management |
| A07:2021 | Identification and Authentication Failures | Authentication, session management, account recovery, MFA |
| A08:2021 | Software and Data Integrity Failures | Trusted updates, CI/CD integrity, code and artifact provenance |
| A09:2021 | Security Logging and Monitoring Failures | Audit trails, alerting, log protection, incident detection |
| A10:2021 | Server-Side Request Forgery (SSRF) | Outbound request controls, destination validation, network restrictions |

## How to apply this reference

1. Identify which categories are relevant to the system architecture and data flows.
2. Map each relevant category to one or more checklist controls.
3. Record evidence and gaps; do not mark a category secure based only on the absence of known incidents.
4. Document compensating controls and residual risks.
5. Prioritize remediation based on business impact and likelihood.

**Reference:** OWASP Top 10:2021 — https://owasp.org/Top10/

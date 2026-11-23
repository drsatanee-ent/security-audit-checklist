# Risk Assessment Methodology

Use this simple qualitative model to prioritize findings. Define assumptions and tailor thresholds to the organization before using it in a real assessment.

## 1. Likelihood

| Score | Rating | Guidance |
|---:|---|---|
| 1 | Rare | Exploitation is difficult and requires unusual conditions |
| 2 | Unlikely | Exploitation is possible but significant barriers exist |
| 3 | Possible | A realistic attack path exists under some conditions |
| 4 | Likely | Exploitation is relatively straightforward or conditions are common |
| 5 | Almost Certain | Exploitation is readily repeatable or already observed |

## 2. Impact

| Score | Rating | Guidance |
|---:|---|---|
| 1 | Insignificant | Minimal operational or data impact |
| 2 | Minor | Limited impact, readily recoverable |
| 3 | Moderate | Noticeable service, confidentiality, or integrity impact |
| 4 | Major | Significant disruption, sensitive data exposure, or financial impact |
| 5 | Severe | Critical service disruption, extensive sensitive-data compromise, or serious safety/legal impact |

## 3. Risk score

**Risk score = Likelihood × Impact**

| Score | Suggested level | Suggested response |
|---:|---|---|
| 1–4 | Low | Track and address through routine improvement |
| 5–9 | Medium | Plan remediation with an assigned owner |
| 10–16 | High | Prioritize remediation and define a target date |
| 17–25 | Critical | Escalate promptly; consider containment or compensating controls |

The score is a prioritization aid, not a precise measurement of risk. Document the rationale behind each score.

## 4. Risk register template

| ID | Finding | Asset | Evidence | Likelihood (1–5) | Impact (1–5) | Score | Level | Owner | Target date | Status |
|---|---|---|---|---:|---:|---:|---|---|---|---|
| R-01 | Example: excessive access permissions | Admin portal | E-01 | 3 | 4 | 12 | High | System owner | TBD | Open |

Replace the example with evidence-based findings before presenting the register as an assessment result.

## 5. Finding record

For each finding, document:

- **Title and ID**
- **Affected asset and environment**
- **Description:** what was observed and why it matters
- **Evidence:** sanitized reference, date, and collection method
- **Impact:** confidentiality, integrity, availability, privacy, and operational effects
- **Likelihood rationale**
- **Risk score and level**
- **Recommended remediation**
- **Responsible owner and target date**
- **Retest method and closure evidence**
- **Residual risk and formal acceptance**, if applicable

## 6. Remediation tracking

Track findings as Open, In Progress, Ready for Retest, Closed, or Risk Accepted. Close a finding only after the agreed remediation has been verified. Risk acceptance should be documented by an authorized risk owner with a review date.

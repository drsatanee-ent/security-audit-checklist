# Security Audit Checklist

Use this checklist for an authorized review. Record evidence, owner, and remediation notes for every control. Select one status: **Pass / Fail / Needs Review / Not Applicable**.

## 1. Governance and scope

- [ ] Assessment authorization and system owner are documented.
- [ ] In-scope applications, APIs, environments, and IP ranges are identified.
- [ ] Out-of-scope assets and prohibited test activities are documented.
- [ ] Data classification and applicable retention requirements are known.
- [ ] System architecture, data flows, and key dependencies are documented.
- [ ] Third-party services and shared-responsibility boundaries are identified.

## 2. Identity, authentication, and access control

- [ ] Unique user identities are used; shared accounts are restricted and controlled.
- [ ] Password policy and secure password storage are implemented.
- [ ] Multi-factor authentication is enabled for privileged and sensitive access.
- [ ] Account recovery and password-reset flows resist account takeover.
- [ ] Login attempts are rate-limited and suspicious activity is monitored.
- [ ] Authorization is enforced server-side on every protected operation.
- [ ] Users receive least-privilege access based on job requirements.
- [ ] Privileged access is reviewed periodically and promptly revoked when no longer needed.
- [ ] Session identifiers are unpredictable and protected.
- [ ] Sessions expire appropriately and logout invalidates the session.
- [ ] Cookie security attributes (Secure, HttpOnly, and appropriate SameSite) are configured.

## 3. Application security and input handling

- [ ] All untrusted input is validated using server-side allowlists where practical.
- [ ] Database access uses parameterized queries or safe ORM mechanisms.
- [ ] Output encoding is context-appropriate to mitigate cross-site scripting (XSS).
- [ ] State-changing requests are protected against cross-site request forgery (CSRF), where applicable.
- [ ] File uploads validate type, size, content, and storage location.
- [ ] Error messages do not expose stack traces, secrets, or internal implementation details.
- [ ] Security-sensitive business rules are enforced on the server.
- [ ] Dependencies and frameworks are maintained and checked for known vulnerabilities.
- [ ] Security headers are configured appropriately for the application.

## 4. API security

- [ ] API endpoints require authentication where appropriate.
- [ ] Object-level and function-level authorization are enforced.
- [ ] Input schemas, types, lengths, and content are validated.
- [ ] Rate limits and resource-consumption limits are applied.
- [ ] Sensitive data is not unnecessarily exposed in responses.
- [ ] CORS allows only approved origins and methods.
- [ ] API keys and tokens are stored securely, rotated, and never committed to source control.
- [ ] Deprecated endpoints and excessive data exposure are addressed.
- [ ] API errors do not disclose sensitive internal details.

## 5. Data protection and cryptography

- [ ] Sensitive data is classified and collected only when necessary.
- [ ] Data in transit is protected using current TLS configurations.
- [ ] Sensitive data at rest is encrypted where required by risk and policy.
- [ ] Cryptographic algorithms and libraries are current and appropriately configured.
- [ ] Passwords are hashed using a purpose-built password-hashing algorithm with salts.
- [ ] Encryption keys and secrets are stored separately from application code and data.
- [ ] Key access, rotation, backup, and revocation processes are documented.
- [ ] Sensitive data is masked or redacted in logs and user interfaces.
- [ ] Data retention and secure deletion processes are defined.

## 6. Server, network, and database security

- [ ] Operating systems, runtimes, and server software receive security updates.
- [ ] Unnecessary services, ports, and default accounts are disabled.
- [ ] Administrative interfaces are restricted to approved networks or access paths.
- [ ] Network segmentation limits access between application tiers.
- [ ] Firewalls and security groups follow least-privilege rules.
- [ ] Database accounts use least privilege and are not shared unnecessarily.
- [ ] Databases are not exposed directly to the public internet unless explicitly justified and protected.
- [ ] Default credentials are changed or disabled.
- [ ] Backups are encrypted, access-controlled, and restoration-tested.
- [ ] Configuration files and deployment environments do not expose secrets.

## 7. Logging, monitoring, and incident response

- [ ] Authentication events and privileged actions are logged.
- [ ] Logs capture sufficient context without recording passwords, tokens, or sensitive payloads.
- [ ] Logs are access-controlled and protected against unauthorized alteration.
- [ ] Alerts exist for suspicious authentication and administrative activity.
- [ ] Time synchronization supports reliable event correlation.
- [ ] Incident response roles, escalation paths, and communication procedures are documented.
- [ ] Security incidents are recorded and reviewed for lessons learned.

## 8. Secure development and operations

- [ ] Code changes receive peer review.
- [ ] Security requirements are considered during design and development.
- [ ] Static analysis and dependency checks are integrated where feasible.
- [ ] Secrets scanning is performed before code is merged.
- [ ] Production and non-production environments are appropriately separated.
- [ ] Deployment permissions are restricted and auditable.
- [ ] Vulnerabilities are tracked to remediation and verified closure.
- [ ] Security configuration changes are reviewed and documented.

## Findings summary

| Control area | Pass | Fail | Needs Review | N/A |
|---|---:|---:|---:|---:|
| Governance and scope |  |  |  |  |
| Identity and access |  |  |  |  |
| Application security |  |  |  |  |
| API security |  |  |  |  |
| Data protection |  |  |  |  |
| Infrastructure and database |  |  |  |  |
| Logging and incident response |  |  |  |  |
| Secure development |  |  |  |  |

**Evidence note:** Reference evidence by identifier (for example, E-01) and store it in an approved, access-controlled location. Never place credentials, private keys, personal data, or confidential production records in this public repository.

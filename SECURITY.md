# Security Policy

## Reporting Security Vulnerabilities

**Do NOT open a public GitHub issue for security vulnerabilities.**

If you discover a security vulnerability in Nudg, please report it privately by emailing:

**security@nudg.com**

### What to Include

- **Type of vulnerability** (e.g., SQL injection, XSS, authentication bypass, data exposure)
- **Location** in the codebase (file path, line numbers if applicable)
- **Description** of the vulnerability and potential impact
- **Proof of concept** or steps to reproduce
- **Suggested fix** (if you have one)
- **Your contact information** and PGP key (if available)

### Response Timeline

- **Acknowledgment**: Within 24 hours
- **Initial Assessment**: Within 72 hours
- **Fix & Patch**: Dependent on severity (see below)
- **Public Disclosure**: After patch is released

---

## Severity Levels & Response Times

| Severity | Description | Response Time | Fix Timeline |
|----------|-------------|----------------|--------------|
| **Critical** | Immediate risk to patient safety or data breach | 6-8 hours | 24-48 hours |
| **High** | Significant security impact, authentication/authorization bypass | 24 hours | 3-5 days |
| **Medium** | Moderate security concern, requires specific conditions | 48 hours | 1-2 weeks |
| **Low** | Minor issue, low exploitability | 1 week | 1 month |

---

## Security Standards & Compliance

### Data Protection
- ✅ **HIPAA Compliant** - All patient data encrypted at rest and in transit
- ✅ **GDPR Compliant** - User data controls and privacy standards implemented
- ✅ **SOC 2 Type II** - Annual security audits and compliance attestation
- ✅ **End-to-End Encryption** - Sensitive data encrypted with AES-256

### Authentication & Authorization
- OAuth 2.0 with PKCE for secure authentication
- Multi-factor authentication (MFA) support
- Role-based access control (RBAC)
- Session management with secure tokens
- No storing of plain-text passwords

### API Security
- TLS 1.2+ for all communications
- API key rotation policies
- Rate limiting on all endpoints
- CORS properly configured
- Input validation and sanitization
- SQL parameterized queries

### Infrastructure
- Infrastructure as Code (IaC) security scanning
- Regular penetration testing
- Vulnerability scanning in CI/CD pipeline
- Dependency checking for known vulnerabilities
- Secrets management (no hardcoded credentials)

---

## Development Security Practices

### Code Review
- All code changes reviewed by at least one maintainer
- Security-focused code reviews for sensitive areas
- Automated security scanning in CI/CD

### Testing
- Unit tests for security functions
- Integration tests for authentication/authorization
- OWASP Top 10 vulnerability scanning
- Dependency vulnerability scanning

### Dependencies
- Regular dependency updates
- Vulnerability monitoring (Snyk, Dependabot)
- Minimal and vetted third-party libraries
- Regular audits of supply chain security

---

## Known Security Considerations

### For Users
- Never share your authentication token or password
- Use strong, unique passwords
- Enable two-factor authentication
- Be cautious of phishing emails claiming to be from Nudg
- Report suspicious account activity immediately

### For Developers
- Never commit secrets (API keys, tokens, passwords)
- Use `.env` files with example `.env.example`
- Implement input validation on all user inputs
- Use parameterized queries for database operations
- Implement proper logging (without logging sensitive data)
- Follow OWASP security guidelines

---

## Privacy & Data Handling

### What We Collect
- User account information (email, name, optional health data)
- Medication adherence data (doses taken, timing)
- Device information for notifications
- Usage analytics (anonymized)

### What We Don't Collect
- Genetic information
- Detailed medical history (unless provided by user)
- Location data (unless explicitly enabled)
- Marketing data for third parties

### Data Retention
- Active user data: Retained as long as account is active
- Deleted accounts: Data deleted within 30 days
- Backups: Retained per compliance requirements
- Audit logs: Retained for 12 months

### User Rights
- Right to access your data
- Right to correct inaccurate data
- Right to delete your account
- Right to data portability
- Right to opt-out of non-essential processing

---

## Incident Response Plan

If a security incident occurs:

1. **Detection & Assessment** (Immediate)
   - Identify the type and scope of incident
   - Assess impact on patient safety and data
   - Activate incident response team

2. **Containment** (Within 4 hours)
   - Isolate affected systems
   - Prevent further unauthorized access
   - Preserve evidence for investigation

3. **Eradication** (24-72 hours)
   - Remove malicious code or access
   - Patch vulnerabilities
   - Fix underlying causes

4. **Recovery** (24-48 hours)
   - Restore systems from clean backups
   - Monitor for signs of re-compromise
   - Verify system integrity

5. **Communication** (Immediate for critical incidents)
   - Notify affected users
   - Inform regulatory bodies if required (HIPAA)
   - Provide guidance on protective measures
   - Publish postmortem and remediation steps

6. **Post-Incident** (1-2 weeks)
   - Complete investigation
   - Implement preventive measures
   - Update security policies
   - Conduct team training

---

## Security Updates & Patches

### Release Process
- Security patches released as soon as possible after fix
- Pre-announcement to critical users (if applicable)
- Public disclosure after patch is available
- All customers notified via email

### Supported Versions
- Latest version: Full support
- Previous major version: Security patches only
- Older versions: Best-effort support

---

## Third-Party Security

### Vendors & Partners
- Vet all third-party services for security compliance
- Require data processing agreements (DPAs)
- Regular security assessments of vendors
- Minimal data sharing, data minimization principle

### Open Source
- Regular monitoring of dependencies for vulnerabilities
- Use tools: Snyk, GitHub Dependabot, npm audit
- Contribute security fixes back to community
- Credit researchers responsibly

---

## Compliance Audits

- **Annual SOC 2 Type II audit**
- **Annual HIPAA compliance review**
- **Quarterly vulnerability assessments**
- **Monthly dependency scanning**
- **Continuous security monitoring**

---

## Contact

- **Security Team**: security@nudg.com
- **General Questions**: support@nudg.com
- **Legal/Compliance**: legal@nudg.com

---

## Acknowledgments

We thank the security research community for helping keep Nudg safe. Researchers who report vulnerabilities responsibly will be credited (with permission) in our security advisories and acknowledgments page.

---

**Last Updated**: September 2024  
**Policy Version**: 1.0


# Security Policy

**Version:** 2.4  
**Last updated:** 2026-02-01  
**Owner:** Platform Security Team  
**Review cycle:** Quarterly

---

## Scope

This policy applies to all NovaDeploy infrastructure, services, and personnel with access to production systems.

---

## Access Control

| Rule | Requirement |
|---|---|
| Production access | Requires MFA and a named approval |
| Service accounts | Rotate credentials every 90 days |
| Offboarding | Access revoked within 24 hours of departure |
| Least privilege | Every role is scoped to minimum required permissions |

No shared credentials. No standing root access.

---

## Deployment Requirements

Every production deployment must:

1. Pass all automated tests in CI
2. Be reviewed by at least one engineer outside the authoring team
3. Be traceable to a Git commit with a signed tag
4. Complete a health check before traffic is routed

Rollbacks are always available. Any engineer on-call can trigger one without approval.

---

## Data Handling

- Customer data is encrypted at rest (AES-256) and in transit (TLS 1.3+)
- Logs are retained for 90 days, then purged
- No customer data is used in test or staging environments
- Personal data handling follows GDPR Article 25 (privacy by design)

---

## Incident Response

| Severity | Response time | Escalation |
|---|---|---|
| P1 — Service down | 15 minutes | CTO + on-call lead |
| P2 — Degraded performance | 1 hour | On-call lead |
| P3 — Non-critical issue | Next business day | Owning team |

All P1 and P2 incidents require a written post-mortem within 5 business days.

---

## Audit Trail

Every change to a production system is logged with:

- Timestamp
- Actor (user or service account)
- Action taken
- Linked deployment or ticket reference

Audit logs are immutable and stored separately from application logs.

---

## Certifications

| Standard | Status |
|---|---|
| SOC 2 Type II | ✅ Certified — renewed January 2026 |
| ISO 27001 | ✅ Certified |
| GDPR | ✅ Compliant |
| Cloud Fortified (Atlassian) | ✅ Listed |

---

## Exceptions

Any exception to this policy requires written approval from the Head of Security and must be documented in the exceptions register with an expiry date.

Undocumented exceptions are treated as violations.

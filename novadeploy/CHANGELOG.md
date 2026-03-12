# Changelog

All notable changes to the NovaDeploy platform are documented here.  
Format follows [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).

---

## [2.4.0] — 2026-03-10

### Added
- Rollback now available directly from the Confluence deployment page via GfC macro
- Support for multi-region deployments (EU-West, US-East, AP-Southeast)
- Webhook events for deployment start, success, and failure

### Changed
- Health check timeout increased from 30s to 60s for large services
- API rate limits raised to 1,000 requests/minute per team

### Fixed
- Service status incorrectly showing "deploying" after a completed rollback
- Environment variable changes not triggering a redeploy when expected

---

## [2.3.2] — 2026-02-14

### Fixed
- Staging promotion blocked when CI pipeline used parallel test runners
- Log timestamps showing UTC offset incorrectly for EU-hosted instances

---

## [2.3.0] — 2026-01-20

### Added
- OpenAPI spec rendering in Confluence via Git for Confluence integration
- Audit log export to CSV for compliance reporting

### Changed
- Default branch for new services changed from `master` to `main`
- Dashboard load time reduced by 40% after caching layer refactor

---

## [2.2.1] — 2025-12-05

### Fixed
- Container startup failures when environment variables contained special characters
- CLI `deploy --dry-run` flag not respecting environment filter

---

## [2.2.0] — 2025-11-18

### Added
- SOC 2 Type II certification (see `compliance/security-policy.md`)
- Per-service scaling rules configurable via `novadeploy.yaml`
- Email notifications for P1 incidents

### Changed
- Minimum supported CLI version bumped to 3.0

---

## [2.1.0] — 2025-10-01

### Added
- Initial managed access support — one token, org-wide read access
- Mermaid and PlantUML diagram rendering in embedded docs

### Deprecated
- Individual Git credentials for embedded content (removed in 2.3.0)

# NovaDeploy Platform

NovaDeploy is a cloud infrastructure platform that lets engineering teams deploy, monitor, and scale services without managing underlying infrastructure.

---

## What it does

- **Deploy** — push code, NovaDeploy handles provisioning, containers, and routing
- **Monitor** — built-in metrics, logs, and alerting per service
- **Scale** — auto-scaling rules based on traffic or custom thresholds
- **Rollback** — one-click rollback to any previous deployment

---

## How teams use it

| Team | What they do |
|---|---|
| Backend | Deploy services, manage environment variables, set scaling rules |
| Frontend | Deploy static builds and edge functions |
| Platform | Manage infrastructure, set quotas, handle access |
| On-call | Monitor dashboards, trigger rollbacks |

---

## Core concepts

**Service** — the unit of deployment. One repo, one service. Each service has its own config, environment, and scaling rules.

**Environment** — services run in `development`, `staging`, or `production`. Promotion between environments is explicit and logged.

**Release** — every deployment creates a release. Releases are versioned, auditable, and reversible.

---

## Getting started

1. Connect your Git repo in the NovaDeploy dashboard
2. Add a `novadeploy.yaml` config to your repo root
3. Push to `main` — your first deployment runs automatically

Full setup guide: [docs.novadeploy.io/quickstart](https://docs.novadeploy.io/quickstart)

---

## Status

| Component | Status |
|---|---|
| API | ✅ Stable |
| CLI | ✅ Stable |
| Dashboard | ✅ Stable |
| Webhooks | 🔧 Beta |
| Terraform provider | 🔧 Beta |

# 90-Day Apprenticeship Progress Tracker

## Overview
- **Start Date:** 2026-06-10
- **Target End Date:** 2026-09-08
- **Current Phase:** Phase 1 - Operations Foundation
- **Current Week:** Week 1
- **Integrated System:** Tenura (repo: `~/Nestera`) — the real application this apprenticeship deploys, operates, monitors, and supports (Project 0)

## Operating Model: Four Tracks
| Track | Focus | Evidence lives in |
|:---|:---|:---|
| **A — Tenura deployment & operations** | Render/Vercel deploys, env vars, health checks, rollback | `Nestera/docs/ops/` + deployment logs |
| **B — Linux & production support curriculum** | Multipass labs, Bash, logs, processes, services | This repo (`week-NN/`, handbook) |
| **C — Incident library & runbooks** | Incidents from labs AND Tenura, RCAs, severity calls | `technical-incident-library/` (canonical) |
| **D — Career artifacts** | Resume bullets, LinkedIn, STAR stories, mock interviews | This repo + tracker |

---

## Phase 1: Operations Foundation (Days 1-30)

### Week 1: Linux Fundamentals & Production Support Mindset

| Day | Topic | Lab Completed? | Artifact Committed? | Proof Sent? |
|:---|:---|:---:|:---:|:---:|
| 1 | Environment Setup & System Baseline | ⬜ | ⬜ | ⬜ |
| 2 | Files, Directories, Permissions | ⬜ | ⬜ | ⬜ |
| 3 | Processes & Resource Inspection | ⬜ | ⬜ | ⬜ |
| 4 | Log Analysis & Evidence Collection | ⬜ | ⬜ | ⬜ |
| 5 | Service Management (systemd) | ⬜ | ⬜ | ⬜ |
| 6 | Bash Health-Check Script | ⬜ | ⬜ | ⬜ |
| 7 | Weekly Review & Mock Interview | ⬜ | ⬜ | ⬜ |

**Week 1 Artifacts Checklist:**
- [ ] `week-01-linux-incident-basics/notes/linux-environment-baseline.md`
- [ ] `technical-incident-library/incident-001-permission-error.md`
- [ ] `technical-incident-library/incident-002-database-connection-failure.md`
- [ ] `linux-operations-handbook/process-management.md`
- [ ] `linux-operations-handbook/service-management.md`
- [ ] `week-01-linux-incident-basics/scripts/syscheck.sh`
- [x] `progress-tracker.md` (this file)

**Week 1 Mock Interview Completed:** ⬜

### Week 2: TBD

| Day | Topic | Lab Completed? | Artifact Committed? | Proof Sent? |
|:---|:---|:---:|:---:|:---:|
| 1 | | ⬜ | ⬜ | ⬜ |

---

## Skills Progress Matrix

Update at end of each week. Scale: 🔴 None | 🟡 Beginner | 🟠 Practicing | 🟢 Portfolio-Ready

| Skill Area | Week 1 | Week 4 | Week 8 | Week 12 |
|:---|:---:|:---:|:---:|:---:|
| Linux Command Line | 🔴 | | | |
| Log Analysis | 🔴 | | | |
| Incident Triage | 🔴 | | | |
| Bash Scripting | 🔴 | | | |
| Service Management | 🔴 | | | |
| API Troubleshooting | 🔴 | | | |
| SQL Troubleshooting | 🔴 | | | |
| Networking for Support | 🔴 | | | |
| Monitoring/Alerting | 🔴 | | | |
| RCA Documentation | 🔴 | | | |
| Interview Readiness | 🔴 | | | |

---

## Portfolio Projects Status

| Project | Phase | Status | Location |
|:---|:---|:---|:---|
| **Project 0: Tenura Production Support Deployment** | 1–3 | In Progress | `Nestera/docs/ops/` + this repo |
| Linux Operations Handbook | 1 | In Progress | `linux-operations-handbook/` |
| Technical Incident Library | 1 | In Progress | `technical-incident-library/` |
| Incident Management Simulator | 2 | Not Started | `incident-management-simulator/` |
| Application Monitoring Dashboard (dual mode: VM metrics + Tenura health) | 3 | Not Started | `application-monitoring-dashboard/` |

---

## Project 0: Tenura PR Plan

| PR | Branch | Scope | Status |
|:---|:---|:---|:---|
| PR-01 | `docs/ops-foundation` | Support overview, env var map, deployment runbook, rollback plan, severity matrix, public-readiness gap analysis (complements existing `docs/runbooks/`) | ⬜ |
| PR-02 | `feat/health-check-startup-validation` | Health endpoint + required env var validation at startup | ⬜ |
| PR-03 | `docs/deployment-evidence-log` | Deployment evidence log + staging validation checklist | ⬜ |
| PR-04 | *(merged into Track C)* | Tenura incidents live in this repo's `technical-incident-library/` (INC-003+) | — |
| PR-05 | `docs/public-trust-foundation` | Privacy/terms drafts, data flow map, legal review TODO | ⬜ |
| PR-06 | `fix/landing-page-proof-aligned-copy` | Claim tightening, privacy/terms placeholders, demo CTA | ⬜ |
| PR-07 | `docs/demo-walkthrough` | Demo script, storyboard, screenshot checklist | ⬜ |

**Tenura incident naming (in `technical-incident-library/`):** INC-003+ with `Environment: Staging / Lab / Simulated` labeled honestly.

---

## Weekly Mentor Check-Ins

| Week | Date Submitted | Proof Format | Mentor Feedback Received? | Advanced to Next Week? |
|:---|:---|:---|:---:|:---:|
| 1 | | | ⬜ | ⬜ |
| 2 | | | ⬜ | ⬜ |
| 3 | | | ⬜ | ⬜ |
| 4 | | | ⬜ | ⬜ |

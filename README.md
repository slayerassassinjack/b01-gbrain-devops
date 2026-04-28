# ☁️ Infrastructure Knowledge Brain

![Domain](https://img.shields.io/badge/Domain-DevOps%20&%20Cloud%20Infrastructure-blue?style=for-the-badge)
![Skills](https://img.shields.io/badge/Skills-8-blue?style=for-the-badge)
![Workflows](https://img.shields.io/badge/Workflows-3-orange?style=for-the-badge)
![Source](https://img.shields.io/badge/Source-gbrain%20(garrytan/gbrain)-grey?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)

> **Self-wiring knowledge graph for infra topology, incident history and runbooks**

Adapted from **gbrain (garrytan/gbrain)** — _self-wiring AI knowledge graph brain — 29 skills, hybrid search, entity enrichment_

---

## What This Does

CI/CD pipelines, container orchestration, IaC, monitoring.

This collection brings the **Infrastructure Knowledge Brain** approach to DevOps & Cloud Infrastructure work,
providing **8 domain-specific skills** and **3 end-to-end workflows**
with structured output and live progress tracking.

---

## Skills

| Skill | Description |
|-------|-------------|
| `/infra-ingest` | Ingest service topology, configs and deployment history into the brain |
| `/incident-ingest` | Store incidents with timeline, root cause, services affected and resolution links |
| `/runbook-query` | Query brain for runbooks, past incidents and resolution patterns |
| `/alert-graph` | Build alert dependency graph: services, metrics, on-call rotations |
| `/cost-brain` | Track cloud spend by service with trend detection and anomaly backlinks |
| `/change-tracker` | Ingest deployment events, config changes and correlate with incidents |
| `/slo-monitor` | Store SLO targets and error budgets, auto-link to incidents on burn |
| `/oncall-brief` | Generate on-call handoff brief from brain: open incidents, recent changes, alerts |

---

## Workflows

| Workflow | Description |
|----------|-------------|
| `infra-brain-init` | Bootstrap: ingest existing runbooks → topology → past incidents → configure crons |
| `incident-response` | During incident: query brain → ingest findings → auto-update runbook |
| `postmortem-brain` | Post-mortem: ingest timeline → extract lessons → update runbooks + entity graph |

---

## UI Preview


```
╔══════════════════════════════════════════════════╗
║  Infra Brain  —  incident query                  ║
╠══════════════════════════════════════════════════╣
║  Searching incident history …     [██████] 100%  ║
║  Traversing service graph …       [██████] 100%  ║
║  Loading runbooks …               [████░░]  67%  ║
╚══════════════════════════════════════════════════╝

3 similar incidents found (P@3 91.2%):
  ① 2025-11-03  api-gateway OOM  → fixed by: increase pod memory limit
  ② 2025-08-17  same pattern     → root cause: memory leak in v2.3.1
  ③ 2025-06-02  related alert    → added circuit-breaker (still active)

💡 Suggested runbook: /runbooks/api-gateway-oom.md
```

---

## How It Works

Every skill follows the same 5-step interaction:

```
① Scope Confirmation   verify target + options
② Live Progress        [████████░░] 80%
③ Structured Findings  table sorted by impact (🔴🟠🟡🟢)
④ Action Plan          quick wins → medium-term → strategic
⑤ Next Steps           suggested follow-up skills
```

---

## Install

```bash
# Copy to Claude skills directory
cp -r . ~/.claude/skills/b01-gbrain--devops/

# Load in Claude Code session
/read ~/.claude/skills/b01-gbrain--devops/SKILL.md
```

## Source

Derived from **gbrain (garrytan/gbrain)** — self-wiring AI knowledge graph brain — 29 skills, hybrid search, entity enrichment.
Original patterns adapted and domain-specialised for DevOps & Cloud Infrastructure.

---
MIT License

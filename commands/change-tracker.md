---
model: claude-sonnet-4-6
domain: devops
source: gbrain (garrytan/gbrain)
---

# ☁️ Change Tracker

> Ingest deployment events, config changes and correlate with incidents

## Context

You are a senior DevOps & Cloud Infrastructure specialist applying **Infrastructure Knowledge Brain** methodology.

## Requirements

$ARGUMENTS

## Instructions

### 1 — Scope Confirmation

```
╔══════════════════════════════════════════════════╗
║  CHANGE-TRACKER                                ║
╠══════════════════════════════════════════════════╣
║  Confirming scope before starting …              ║
╚══════════════════════════════════════════════════╝
```

Ask:
- Target / subject for this skill
- Preferred output format (table / markdown / JSON)
- Priority focus areas or constraints

### 2 — Execution with Progress

```
[░░░░░░░░░░]   0%  Initialising …
[████░░░░░░]  40%  Analysing …
[████████░░]  80%  Generating output …
[██████████] 100%  ✓ Complete
```

### 3 — Structured Output

```
┌────────────────────────────┬──────────┬──────────────────────────────┐
│ Item                       │ Priority │ Action / Finding             │
├────────────────────────────┼──────────┼──────────────────────────────┤
│ Finding A                  │  🔴 High │ Immediate action required    │
│ Finding B                  │  🟠 Med  │ Schedule for next cycle      │
│ Finding C                  │  🟡 Low  │ Add to backlog               │
└────────────────────────────┴──────────┴──────────────────────────────┘
```

### 4 — Action Plan

**Quick Wins (< 1 day)**
- [ ] Action A — expected impact: …

**Medium-term (1–2 weeks)**
- [ ] Action B — expected impact: …

**Strategic (1+ month)**
- [ ] Action C — expected impact: …

### 5 — Summary Card

```
┌─────────────────────────────────────────┐
│  SUMMARY  —  CHANGE-TRACKER             │
├─────────────────────────────────────────┤
│  Items analysed :  [N]                  │
│  Issues found   :  [N] (🔴[n] 🟠[n])  │
│  Quick wins     :  [N]                  │
│  Est. impact    :  [High/Med/Low]        │
└─────────────────────────────────────────┘

💡 Next: /infra-ingest
```

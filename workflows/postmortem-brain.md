---
model: claude-sonnet-4-6
type: workflow
domain: devops
source: gbrain (garrytan/gbrain)
---

# ☁️ Workflow: Postmortem Brain

> Post-mortem: ingest timeline → extract lessons → update runbooks + entity graph

## Overview

End-to-end **DevOps & Cloud Infrastructure** workflow based on the
**Infrastructure Knowledge Brain** approach from _gbrain (garrytan/gbrain)_.

## Start

```bash
/workflows:postmortem-brain [target] [--scope full|quick] [--output md|json|html]
```

## Dashboard

```
╔══════════════════════════════════════════════════════════╗
║  WORKFLOW: POSTMORTEM-BRAIN                             ║
╠══════════════════════════════════════════════════════════╣
║  Step 1/5  Discovery        ✓  Completed                 ║
║  Step 2/5  Analysis         ✓  Completed                 ║
║  Step 3/5  Planning         ⟳  Running …                 ║
║  Step 4/5  Execution        ░  Pending                   ║
║  Step 5/5  Report           ░  Pending                   ║
╠══════════════════════════════════════════════════════════╣
║  [████████████░░░░░░░░]  60%   ETA: ~12 min              ║
╚══════════════════════════════════════════════════════════╝
```

## Completion Report

```markdown
## Postmortem Brain — Report

**Date:** {date}  **Duration:** {duration}

### Summary
{2-3 sentence executive summary}

### Findings
| Priority | Finding | Owner | Due |
|----------|---------|-------|-----|

### Metrics
| Metric | Before | After | Δ |
|--------|--------|-------|---|
```

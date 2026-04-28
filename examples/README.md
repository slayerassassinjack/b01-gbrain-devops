# ☁️ Examples — Infrastructure Knowledge Brain

## Quick Command Example

```bash
/infra-ingest my-target --output md
```

**Output:**


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

## Workflow Example

```bash
/workflows:infra-brain-init my-target --scope full
```

```
╔══════════════════════════════════════════════════════════╗
║  Step 1/5  Discovery   ✓  Done                          ║
║  Step 2/5  Analysis    ✓  Done                          ║
║  Step 3/5  Planning    ⟳  Running …                    ║
║  [████████████░░░░░░]  60%   ETA ~12 min                ║
╚══════════════════════════════════════════════════════════╝
```

## Tips

1. Start with `/infra-ingest` for a quick overview.
2. Use `--scope quick` for fast scans, `--scope full` for production.
3. Chain: run analysis first → use findings as input for planning.
4. `--output html` generates a stakeholder-ready report.

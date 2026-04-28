        ---
        name: "b01-gbrain--devops"
        description: >
          ☁️ Infrastructure Knowledge Brain — Self-wiring knowledge graph for infra topology, incident history and runbooks.
          Derived from gbrain (garrytan/gbrain). CI/CD pipelines, container orchestration, IaC, monitoring.
        version: "1.0.0"
        domain: devops
        tags: ["devops", "cloud", "docker", "kubernetes", "ci-cd"]
        source_concept: "Infrastructure Knowledge Brain"
        license: MIT
        ---

        # ☁️ Infrastructure Knowledge Brain

        > **Self-wiring knowledge graph for infra topology, incident history and runbooks**
        > Derived from _gbrain (garrytan/gbrain)_ — self-wiring AI knowledge graph brain — 29 skills, hybrid search, entity enrichment

        ## Available Skills

        - `/infra-ingest` — Ingest service topology, configs and deployment history into the brain
- `/incident-ingest` — Store incidents with timeline, root cause, services affected and resolution links
- `/runbook-query` — Query brain for runbooks, past incidents and resolution patterns
- `/alert-graph` — Build alert dependency graph: services, metrics, on-call rotations
- `/cost-brain` — Track cloud spend by service with trend detection and anomaly backlinks
- `/change-tracker` — Ingest deployment events, config changes and correlate with incidents
- `/slo-monitor` — Store SLO targets and error budgets, auto-link to incidents on burn
- `/oncall-brief` — Generate on-call handoff brief from brain: open incidents, recent changes, alerts

        ## Interaction Pattern

        ```
        ① Scope    — confirm target, depth and output format
        ② Execute  — live progress with block-character bar
        ③ Findings — structured table sorted by impact
        ④ Actions  — quick wins → medium-term → strategic
        ⑤ Next     — suggested follow-up skill
        ```

        ## UI Conventions

        | Symbol | Meaning          |
        |--------|------------------|
        | ✓      | Pass / complete  |
        | ✗      | Fail / critical  |
        | ⚠      | Warning / review |
        | ⟳      | In progress      |
        | 🔴🟠🟡🟢 | Severity levels |

        Progress: `[████████░░] 80%`

        ## Quick Install

        ```bash
        cp -r . ~/.claude/skills/b01-gbrain--devops/
        # In Claude Code:
        /read ~/.claude/skills/b01-gbrain--devops/SKILL.md
        ```

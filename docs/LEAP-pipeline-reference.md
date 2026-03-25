# LEAP Pipeline Reference
## Implementation spec for engineers and tool builders

---

## Node Types

| Type | Character | Parent | Children | Primary Artifact |
|------|-----------|--------|----------|-----------------|
| `learn` | Abstract — goal & opportunity | Workspace root | `explore` nodes | `strategy.md` |
| `explore` | Creative — solutions & concepts | `learn` | `action` nodes | `product-brief.md` |
| `action` | Tactical — execution & production | `explore` | `prove` nodes | `bet-card.md` |
| `prove` | Evaluative — evidence & decision | `action` | none | `evidence.md` |

**VALID_CHILDREN:** `learn → explore`, `explore → action`, `action → prove`. No skipping levels. Enforced server-side.

---

## Tree Structure

```
WORKSPACE ROOT (learn)
├── strategy.md
├── opportunity-map.md
├── {opportunity}/ ──────── learn node
│   └── {concept}/ ─────── explore node
│       ├── product-brief.md
│       ├── prototype-prd.md
│       └── {bet}/ ─────── action node
│           ├── bet-card.md
│           └── evidence.md ── prove child
```

---

## Stage Lifecycle

### LEARN States
`understand → define`

| Skill | Advances To |
|-------|------------|
| `strategy-sprint` | define |
| `opportunity-discovery` | define |
| `metrics-framework` | define |

### EXPLORE States
`define → decide`

| Skill | Advances To |
|-------|------------|
| `product-brief` | decide |
| `solution-concepts` | decide |
| `risk-assessment` | decide |

### ACTION States
`decide → build`

| Skill | Advances To |
|-------|------------|
| `experiment-design` | build |

### PROVE States
`build → ship`

| Skill | Advances To |
|-------|------------|
| `learning-report` | ship |
| `retrospective` | ship |

---

## Status Machine (unified across all types)
`draft → in_progress → finished → cancelled`

Display labels vary by type:
- LEARN: Draft → Active → Evolved → Archived
- EXPLORE: Diverging → Stress-testing → Recommended → Killed
- ACTION: Planning → Executing → Decided → Killed
- PROVE: Pending → Reviewing → Decided → Archived

---

## PROVE Decision Routing

| Decision | Creates | Placement | Evidence |
|----------|---------|-----------|----------|
| **Ship** | Launch plan | Exits loop | Opportunity marked "validated" in LEARN map |
| **Iterate** | New `action` | Sibling under same `explore` | Inherits bet card, adjusts criteria |
| **Pivot** | New `explore` | Sibling under same `learn` | Old branch marked "tested — approach failed" |
| **Kill** | Nothing | Branch archived | All artifacts preserved. Kill rationale saved. |

Auto-triggers after decision: `opportunity-map-update` + `retrospective`

---

## Context Architecture (5 layers)

| Layer | Scope | Managed By | Slugs |
|-------|-------|-----------|-------|
| L1 Organization | Org-wide | Admin | `company`, `personas`, `goals` |
| L2a Business Line | Domain-specific | Admin | `product`, `personas`, `competitors`, `goals` |
| L2b Market | Market/country | Admin | `product`, `personas`, `competitors`, `goals` |
| L3 Workspace | Workspace-level | PM | `company`, `product`, `personas`, `competitors`, `goals` |
| L4 Personal | PM voice & style | PM | `voice_config` on user record |

**Flow:** L1 → L2a + L2b → L3 → Ancestry → Node docs → Layer guidance

**Propagation:** Learnings climb upward. Parent auto-applied. Deeper ancestors drafted for review.

---

## Skill Catalog (23 skills)

### LEARN (6)
| Slug | Execution | Output |
|------|-----------|--------|
| `strategy-sprint` | parallel-synthesis (3 agents) | strategy.md |
| `opportunity-discovery` | parallel-synthesis | opportunity-map.md |
| `metrics-framework` | single agent | success.md |
| `interview-snapshot` | single agent | 200-word note |
| `signal-synthesis` | parallel-synthesis | weekly digest |
| `opportunity-map-update` | single agent | map update (auto-triggered) |

### EXPLORE (7)
| Slug | Execution | Output |
|------|-----------|--------|
| `solution-concepts` | parallel-synthesis (constraint lenses) | solution cards |
| `product-brief` | parallel-synthesis | product-brief.md |
| `competitive-intel` | parallel-synthesis | competitive analysis |
| `risk-assessment` | single agent | risk register |
| `premortem` | single agent | pre-mortem.md |
| `pressure-test` | parallel-synthesis | devil's advocate |
| `prototype-prd` | single agent | spec + HTML prototype |

### ACTION (4)
| Slug | Execution | Output |
|------|-----------|--------|
| `experiment-design` | interactive (interview) | bet-card.md |
| `sprint-breakdown` | interactive (interview) | HITL/AFK stories |
| `stakeholder-brief` | single agent | 1-page brief |
| `launch-plan` | single agent | GTM plan |

### PROVE (2)
| Slug | Execution | Output |
|------|-----------|--------|
| `learning-report` | single agent | evidence.md + decision |
| `retrospective` | single agent | retrospective.md |

### Cross-cutting (4)
| Slug | Execution | Output |
|------|-----------|--------|
| `apply-framework` | single agent | scored ranking |
| `crisis-response` | single agent | incident comms |
| `quarterly-plan` | single agent | quarterly roadmap |
| `executive-comms` | parallel-synthesis | slides/pre-reads/LinkedIn |

---

## Chains (5 multi-skill sequences)

| Chain | Steps | Start Type |
|-------|-------|-----------|
| `goal-discovery` | competitive-intel → opportunity-discovery → product-brief → prototype-prd → experiment-design | learn |
| `opportunity-deep-dive` | competitive-intel → product-brief → prototype-prd → experiment-design | learn |
| `build-test-learn` | experiment-design → prototype-prd → learning-report | action |
| `result-feedback` | learning-report → experiment-design | prove |
| `ship-and-launch` | launch-plan → sprint-breakdown → stakeholder-brief | action |

---

## Autopilot Execution

Phases adapt based on starting node type:

**From LEARN:** Strategy → Opportunities → Solutions + Prototypes → Experiments → Action Prototypes

**From EXPLORE:** Solutions + Prototypes → Experiments → Action Prototypes

**From ACTION:** Action Prototypes only

Concurrency: 3 EXPLORE pipelines run in parallel. Within each pipeline: brief → prototype → experiment → action prototypes (batched at 3 concurrent).

---

## Quality Gate

| Score | Tier | Action |
|-------|------|--------|
| 70-100 | **Publish** | Becomes a node in the tree |
| 50-69 | **Watch** | Saved as parked doc on parent |
| 0-49 | **Park** | Logged in comments only |

Document quality: every non-prototype output scored by AI reviewer. Below 70 → regenerated once with specific feedback.

---

## Agent Architecture

| Agent | Model | Role |
|-------|-------|------|
| Strategist | Sonnet | Market analysis, competitive positioning, 7 Powers |
| Researcher | Haiku | User patterns, behavioral signals, JTBD |
| Analyst | Haiku | Scenarios, projections, systems impact |
| Builder | Sonnet | Execution plans, PRDs, prototypes |
| Interview | Haiku | Decision-tree Q&A before generation |
| Technical Reviewer | Haiku | Feasibility review |
| User Reviewer | Haiku | Usability review |
| Business Reviewer | Haiku | Viability review |

Parallel-synthesis skills: Strategist + Researcher + Analyst run concurrently → Synthesis agent (Sonnet) merges.

---

## MCP Connectors (7 bundled)

| Server | Purpose | Reference Links |
|--------|---------|----------------|
| GitHub | Competitive intel, code refs | Product repo, competitor repos |
| Slack | Updates, feedback channels | Product channel, feedback channel |
| Google Drive | Strategy docs, research | Strategy doc, OKR sheet, research folder |
| Figma | Design system, prototypes | Design system file, product screens |
| Miro | Workshop outputs | Discovery board, journey map |
| BigQuery | Metrics, experiment results | Events table, orders table, experiments table |
| Filesystem | Local file ingestion | Allowed directories |

Each connector's references are injected into skill prompts automatically.

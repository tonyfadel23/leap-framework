# LEAP: The AI-First Product Discovery System
## Learn · Explore · Action · Prove

> The product roadmap is a graveyard of unvalidated assumptions. LEAP replaces it with a system that makes learning the unit of progress — not the feature, not the sprint, not the story point. The resolved bet.

---

## This is not an improvement to how PMs work. It's a replacement.

Every product tool on the market does the same thing: takes the existing PM workflow and adds AI. Write a PRD faster. Summarize interviews. Auto-generate acceptance criteria. AI as autocomplete for the same broken process.

LEAP was not designed that way. It was designed from scratch as a system where AI is the execution layer and humans are the decision layer. The framework and the AI are architecturally inseparable. Remove the AI and you don't get a simpler framework. You get nothing. Like removing the engine from a car — it's not a slower car, it's a sculpture.

Twenty years of product experience designed the decision architecture. AI designed the execution architecture. LEAP is what happens when both are built at the same time, for the same system, from the ground up.

---

## The Architecture: Three Stages, One Layer

LEAP has three stages and one evaluation layer.

**LEARN**, **EXPLORE**, and **ACTION** are the three stages — sequential in concept, fluid in practice.

**PROVE** is not a stage. It's a continuous evaluation layer that runs across all three. At every point in the loop, PROVE asks: *"Based on what we now know, should we continue, change direction, or stop?"*

```
╔════════════════════════════════════════════════════════════════╗
║  P R O V E   (continuous evaluation layer)                     ║
║  At every stage: Should we continue, change, or stop?          ║
║  Decisions: Ship · Iterate · Pivot · Kill                      ║
║                                                                ║
║  ┌─────────┐       ┌──────────┐       ┌──────────┐           ║
║  │  LEARN  │──────▶│ EXPLORE  │──────▶│  ACTION  │           ║
║  │Abstract │       │ Creative │       │ Tactical │           ║
║  └────┬────┘       └──────────┘       └─────┬────┘           ║
║       │                                      │                ║
║       └──────────── Loop (enriched) ─────────┘                ║
║                                                                ║
║  Ship ──▶ Exits loop → Scale & Operate                        ║
╚════════════════════════════════════════════════════════════════╝
```

---

## LEARN — The Problem Is Not "What Should We Build?"

The problem is: what problem is worth solving, for whom, and why now?

Most teams skip LEARN. They start with a solution idea and work backwards to justify it. Or they do "discovery" — which means talking to five users about a feature they've already decided to build.

LEARN forces ranking before research. Every opportunity is scored by **TAP — Total Addressable Pain:**

**TAP = Reach × Frequency × Intensity**

- **Reach:** % of segment affected (sourced, not guessed)
- **Frequency:** daily > weekly > monthly > rare
- **Intensity:** abandon > frustrate > annoy > notice

TAP, not TAM. Pain drives behavior change. Revenue projections don't.

Then the **Customer Relationship Hierarchy** filters what gets worked on next:

**Functional → Trustworthy → Engaging → Valuable → Loved**

This is Maslow for product. You don't build personalization when search is broken. You don't build delight when customers can't trust your delivery time. Solve the current stage before building for the next.

A team once pitched me a beautiful recommendation engine. I asked: "What relationship stage are we in with this segment?" Functional — customers couldn't find their last order. The hierarchy killed the project in one question. That's LEARN doing its job.

### What LEARN produces:
- **strategy.md** — Narrative, Outcome (metric + baseline + target), Customer Relationship Stage, Guardrails, Target Opportunity
- **opportunity-map.md** — TAP-scored, evidence-tagged, living document

### How AI executes LEARN:
Three agents analyze the same problem space in parallel — Strategist (market lens), Researcher (user lens), Analyst (systems lens). A synthesis agent merges their perspectives. The PM gets a multi-perspective strategy document in minutes that would take a cross-functional team days. The PM's job: critique it, challenge the scoring, and decide which opportunity to pursue.

---

## EXPLORE — Generate Alternatives, Not Confirmations

Not one solution — multiple. At least three. Each materially different enough to test a different assumption.

The engine: **DIVERGE → STRESS-TEST → CONVERGE.**

**Diverge** generates options. **Stress-Test** runs a pre-mortem on each — "It's six months from now and this solution failed. What happened?" Classify the risks: Tigers (real threats), Paper Tigers (fears that dissolve on inspection), Elephants (obvious problems nobody names). **Converge** picks the approach with the best risk-to-signal ratio.

AI changed EXPLORE fundamentally. Two years ago, a prototype took two weeks. Now it takes two hours. You generate five interactive prototypes in a morning and show them to users by lunch. EXPLORE went from bottleneck to accelerator.

### What EXPLORE produces:
- **product-brief.md** — Opportunity (customer voice), Customer Experience (before/after), Why Not (strongest argument against), Recommended Approach, Release Structure, Riskiest Assumptions
- **prototype-prd.md** — Machine-readable spec + working HTML prototype
- **pre-mortem.md** — Tigers, Paper Tigers, Elephants

### How AI executes EXPLORE:
Three constraint-based lenses run in parallel — Speed to Market, Long-term Defensibility, Minimum Viable Effort — then synthesize. The PM picks the approach. Interactive prototypes are generated directly from the brief. No designer bottleneck. No two-week wait. Prototype as thinking tool, not deliverable.

### Rationalisation:
**Compound Prioritisation:** 1) Relationship stage first, 2) Releases over features, 3) CX KPIs over feature KPIs, 4) Opportunity cost.

---

## ACTION — Place the Bet, Define the Kill Criteria

Every solution becomes a bet. Every bet has a size:

| Size | Duration | Confidence Required |
|------|----------|-------------------|
| **Scout** | Hours to 2 days | Low — "we think this might matter" |
| **Sprint** | 1-2 weeks | Medium — "evidence suggests this" |
| **Campaign** | 2-4 weeks | High — "validated in Scout/Sprint" |
| **Moonshot** | 4-8 weeks | Very high — "strategic commitment" |

The size matches your confidence. Low confidence does not get a Campaign. It gets a Scout — four hours, one signal.

The bet card defines four things **before execution starts:**

1. **Hypothesis:** "If we [do X], then [metric Y] will [move by Z]"
2. **Execution plan:** who builds what, by when
3. **Measurement:** primary metric, counter-metrics, duration
4. **Prove criteria:** Ship if A. Iterate if B. Pivot if C. Kill if D.

This is pre-commitment. You are not deciding what to do with the results in the heat of the moment — surrounded by sunk cost bias and organizational pressure to ship. You decided before you started.

### What ACTION produces:
- **bet-card.md** — Context Chain, Bet Definition (size + hypothesis), Execution Plan, Measurement, Prove Criteria
- **execution-log.md** — Running observations during the bet

### How AI executes ACTION:
The interview agent walks a decision tree before generating the bet card — auto-resolving from context vault first, only asking the PM what it can't resolve. The bet card is scored for quality before publishing. Engineers get stories classified as HITL (PM decision needed) or AFK (engineering proceeds autonomously).

---

## PROVE — Not a Phase. A Layer.

This is the insight most frameworks get wrong. PROVE is not the last step. It runs across all three stages simultaneously.

- In **LEARN**, PROVE asks: "Is this still the right opportunity? Has the landscape shifted?"
- In **EXPLORE**, PROVE asks: "Does this prototype survive a stress test? Did users react?"
- In **ACTION**, PROVE asks: "Are we hitting our criteria? Should we ship, iterate, pivot, or kill?"

### Decision Routing

When a bet resolves, the decision routes back through the system:

| Decision | What Happens | Where It Goes |
|----------|-------------|---------------|
| **Ship** | Exit the loop | Scale & Operate. Launch plan created. Opportunity marked "validated." |
| **Iterate** | New bet, same concept | Sibling ACTION under the same EXPLORE. Adjust hypothesis. |
| **Pivot** | New concept, same opportunity | New EXPLORE under the same LEARN. Approach failed, problem still valid. |
| **Kill** | Archive with evidence | Branch preserved. Every artifact, prototype, and evidence saved. |

**The kill is the most valuable outcome.** A kill with evidence saves months of building the wrong thing. The kill rationale becomes organizational memory. Six months later, someone has the same idea, opens the tree, and finds: "We tested this. Here's what happened. Here's why we stopped."

### What PROVE produces:
- **evidence.md** — Hypothesis, Plan, Results (quant + qual + ops), Interpretation, Decision, Routing, Reasoning

---

## The Five Architectural Decisions That Make LEAP AI-First

### 1. Skills, not templates
Traditional frameworks give you a template: fill in the blanks. LEAP gives you skills — AI-powered agents that generate complete artifacts from context. The PM doesn't fill a template. The PM reviews, critiques, and decides. Less writer. More judge.

### 2. Parallel-synthesis, not sequential review
Three agents analyze simultaneously from different lenses, then a synthesis agent merges. This architecture only works with AI. You can't parallelize humans.

### 3. Quality scoring as a filter, not a gate
Every candidate is scored 0-100. Above 70: **publish** to the tree. 50-69: **watch** (parked for later). Below 50: **park** (logged and forgotten). No artificial "generate 3-5" quota. The AI generates all worthy candidates. Quality gates filter automatically.

### 4. Autopilot as the default, not the exception
LEAP runs the entire discovery loop autonomously. Strategy → opportunities → product briefs → prototypes → experiments. The PM reviews at decision points. The AI handles everything between.

### 5. Compound context, not fresh starts
Every cycle enriches the tree. Every resolved bet adds evidence. Every kill adds a rationale. The AI reads all of it before generating anything new. The 10th bet is smarter than the first because it stands on nine previous cycles.

---

## The PM's Role in AI-First LEAP

The PM does not write. The PM decides.

The PM sets the goal. Critiques the strategy. Challenges the opportunity scoring. Picks the bet size. Defines the kill criteria. Makes the ship/iterate/pivot/kill call.

Everything between those decisions — research synthesis, brief generation, prototype creation, quality scoring, evidence compilation — is executed by AI.

This is not a diminishment. It's an elevation. The PM stops being a writer of documents and becomes a judge of decisions. The thinking gets harder, not easier. The decisions get better because the evidence is richer.

---

## The Compound Effect

After three quarters of running LEAP, a team has organizational memory:

| Quarter | Bets Resolved | What Changes |
|---------|--------------|-------------|
| Q1 | 5 | Learning the system. Mostly Scouts. |
| Q2 | 12 | Each bet starts with Q1's evidence. Kill decisions take days, not weeks. |
| Q3 | 18+ | The compound flywheel is spinning. New bets inherit 50+ previous evidence artifacts. |

**More resolved bets → more evidence → better-informed future bets → faster resolution → more resolved bets.**

The metric that matters: **bets resolved per quarter.** Not features shipped. A team resolving 15 bets with evidence will outperform a team shipping 50 features without signal. Every single time.

---

## The 5-Layer Context Architecture

LEAP doesn't start from scratch. It inherits context:

| Layer | What | Managed By |
|-------|------|-----------|
| **L1 Organization** | Company, personas, goals | Admin |
| **L2a Business Line** | Product, competitors, domain | Admin |
| **L2b Market** | Market-specific context | Admin |
| **L3 Workspace** | Workspace overrides, vault | PM |
| **L4 Personal** | PM's voice and style | PM |

Context flows downward: L1 → L2 → L3 → L4 → Node. Learnings propagate upward. Parent nodes auto-update when children resolve. The tree is alive.

---

## What to Do Monday Morning

1. Pick one goal. Write it as a metric with a baseline and a target.
2. Map three opportunities by TAP. Pick the highest-pain one.
3. Generate three solutions. Pre-mortem each in 30 minutes.
4. Build a Scout bet. Define the hypothesis and the kill criteria.
5. Resolve it by Friday.

The system sells itself after the first kill. That's when the team realizes they saved three months of building the wrong thing. And they have the evidence to prove it.

---

## What This Is Not

**Not a replacement for customer empathy.** AI accelerates execution. It does not replace the judgment that comes from sitting with a customer and watching them struggle. The PM's job is to decide — and good decisions require deep understanding.

**Not a linear process.** L→E→A looks sequential. In practice, PROVE sends you back constantly. A killed bet sends you to LEARN. A pivoted concept sends you to EXPLORE. The tree is the system of record — not a Gantt chart.

**Not a framework for teaching purposes only.** LEAP is operationalized — it runs as software with real nodes, agents, and quality gates. But the moment you follow the stages mechanically without engaging your judgment, you've built a feature factory with better labels.

**Not a way to avoid accountability.** When AI generates and the PM decides, the PM owns the outcome. The four risks (value, usability, feasibility, viability) still need a human accountable for each one. AI makes the evidence richer. The human still makes the call.

---

*Build less. Learn more. Let the AI execute. You decide.*

---

*Tony Fadel · CPO · 20+ years in product · Building from the UAE · Software has no soil conditions.*

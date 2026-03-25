# LEAP: AI-First Product Discovery System

**Learn · Explore · Action · Prove**

> The product roadmap is a graveyard of unvalidated assumptions. LEAP replaces it with a system that makes learning the unit of progress — not the feature, not the sprint, not the story point. The resolved bet.

---

## What is LEAP?

LEAP is an AI-first product discovery system. Three stages, one continuous evaluation layer. AI executes the research, prototyping, and evidence gathering. The PM's job is to decide: **ship, iterate, pivot, or kill.**

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

### This is not AI-augmented product management. It's AI-first.

Every product tool on the market takes the existing PM workflow and adds AI. Write a PRD faster. Summarize interviews. AI as autocomplete for the same broken process.

LEAP was designed from scratch assuming AI exists. Remove the AI and you don't get a simpler framework. You get nothing. Like removing the engine from a car — it's not a slower car, it's a sculpture.

---

## The Three Stages

### LEARN — What problem is worth solving?
Score opportunities by **TAP (Total Addressable Pain)** = Reach × Frequency × Intensity. Filter by the **Customer Relationship Hierarchy**: Functional → Trustworthy → Engaging → Valuable → Loved. Solve the current stage before building for the next.

### EXPLORE — Generate alternatives, not confirmations
At least three solutions. **Diverge → Stress-Test → Converge.** Pre-mortem each: Tigers (real threats), Paper Tigers (false fears), Elephants (nobody's saying it). AI generates interactive prototypes in hours, not weeks.

### ACTION — Place the bet, define the kill criteria
Every solution becomes a bet: **Scout** (hours) · **Sprint** (1-2 weeks) · **Campaign** (2-4 weeks) · **Moonshot** (4-8 weeks). Size matches confidence. Pre-commit prove criteria: ship if X, iterate if Y, pivot if Z, kill if W.

### PROVE — Not a phase. A layer.
Runs across all three stages. When a bet resolves: **Ship** exits the loop. **Iterate** creates a sibling bet. **Pivot** creates a new concept. **Kill** archives with evidence — the most valuable outcome.

---

## The Five Architectural Decisions

| Decision | What It Means |
|----------|--------------|
| **Skills, not templates** | AI agents generate artifacts from context. PM reviews and decides. |
| **Parallel-synthesis** | 3 agents analyze simultaneously, synthesis agent merges. |
| **Quality scoring** | Every artifact scored 0-100. Publish (≥70), Watch (50-69), Park (<50). |
| **Autopilot** | Full discovery loop runs autonomously. PM reviews at decision points. |
| **Compound context** | Every cycle enriches the tree. The 10th bet is smarter than the first. |

---

## The Metric That Matters

**Bets resolved per quarter.** Not features shipped.

A team resolving 15 bets with evidence will outperform a team shipping 50 features without signal. Every single time.

---

## Documents

| Document | Description |
|----------|-------------|
| [**LEAP Framework**](docs/LEAP-framework.md) | The canonical reference — full framework with all stages, tools, and architecture |
| [**AI-First Positioning**](docs/LEAP-ai-first.md) | Why LEAP is AI-first, not AI-augmented |
| [**Anti-Patterns**](docs/LEAP-anti-patterns.md) | The 7 product diseases LEAP was built to kill |
| [**Benchmarks**](docs/LEAP-benchmarks.md) | What good looks like — bets resolved, kill rates, TAP scoring |
| [**Onboarding Guide**](docs/LEAP-onboarding.md) | 90-day rollout for PMs and engineers |
| [**Pipeline Reference**](docs/LEAP-pipeline-reference.md) | Implementation spec for engineers and tool builders |
| [**Elevator Pitch**](docs/LEAP-elevator-pitch.md) | 15-second, 60-second, and 3-minute versions |
| [**Substack Essay**](docs/LEAP-substack-essay.md) | Long-form essay for Medium/Substack |
| [**LinkedIn Series**](docs/LEAP-linkedin-series.md) | 7-post series optimized for virality |
| [**Podcast Transcript**](docs/LEAP-lenny-podcast.md) | Simulated Lenny's Podcast conversation |

---

## Quick Start

1. Pick one goal. Write it as a metric: baseline → target → deadline.
2. Map three opportunities by TAP. Pick the highest-pain one.
3. Generate three solutions. Pre-mortem each in 30 minutes.
4. Build a Scout bet. Define the hypothesis and the kill criteria.
5. Resolve it by Friday.

The system sells itself after the first kill.

---

## Key Concepts

- **TAP** — Total Addressable Pain (Reach × Frequency × Intensity)
- **Customer Relationship Hierarchy** — Functional → Trustworthy → Engaging → Valuable → Loved
- **Bet Sizing** — Scout · Sprint · Campaign · Moonshot
- **Quality Gate** — Publish (≥70) · Watch (50-69) · Park (<50)
- **Decision Routing** — Ship · Iterate · Pivot · Kill

---

## Who Made This

**Tony Fadel** — CPO with 20+ years in product leadership. Currently leading a 500-person product and tech org at Talabat/Delivery Hero. Building from the UAE.

I believe software has no soil conditions. World-class product teams can be built anywhere.

---

## License

This work is licensed under [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/). Share it, adapt it, build on it — just credit the source and share alike.

---

*Build less. Learn more. Let the AI execute. You decide.*

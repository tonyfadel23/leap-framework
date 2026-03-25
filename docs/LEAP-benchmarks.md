# LEAP Benchmarks: What Good Looks Like

> Numbers without context are noise. These benchmarks are drawn from how LEAP teams actually perform — not aspirational targets, but observed patterns across teams running the system. Use them to calibrate, not to punish.

---

## Bets Resolved Per Quarter

The unit of progress is the resolved bet. Not features shipped. Not story points burned. A resolved bet means: hypothesis stated, experiment run, evidence collected, decision made. Ship, iterate, pivot, or kill.

| Team Maturity | Bets Resolved / Quarter | What It Looks Like |
|---|---|---|
| **Quarter 1** (learning the system) | 4–6 | Mostly Scouts. Teams are calibrating bet sizing and learning to write kill criteria before execution. Expect false starts. |
| **Quarter 2** (building rhythm) | 10–14 | Each bet starts with Q1's evidence. Kill decisions take days, not weeks. First Campaigns appear. |
| **Quarter 3** (compound flywheel) | 16–22 | New bets inherit 50+ previous evidence artifacts. Teams resolve faster because the tree is richer. Sprint-to-Ship conversion improves. |
| **Quarter 4+** (operating cadence) | 20–30 | Bets resolve in parallel across multiple opportunity branches. The AI contextualizes at speed. Discovery becomes continuous, not periodic. |

A team resolving fewer than 4 bets per quarter is not running LEAP. They are running a traditional roadmap with LEAP labels.

---

## Healthy Kill Rate

A kill rate of zero means nobody is testing assumptions — they are shipping features. A kill rate above 50% means the team is placing bets without enough signal. Both are diseases.

| Kill Rate | What It Means | Action |
|---|---|---|
| **0–15%** | Everything ships. Nobody is testing hard enough. Hypotheses are too safe or kill criteria are too lenient. | Tighten kill criteria. Increase Scout bets on riskier assumptions. |
| **15–29%** | Cautious but learning. Healthy for Q1 teams still building the muscle. | Push toward more divergent EXPLORE. Generate more alternatives. |
| **30–40%** | The healthy range. The team is placing real bets on real unknowns and killing what doesn't work. Evidence compounds. | Maintain. This is the signal that LEAP is operating as designed. |
| **41–50%** | Aggressive but productive. Common in teams exploring new markets or running many Scouts. | Watch for fatigue. Ensure kills are producing learnings, not just volume. |
| **50%+** | Too many bets are failing. Either bet sizing is wrong (Campaigns where Scouts should be) or opportunity scoring is broken. | Recalibrate TAP scoring. Check whether LEARN is being skipped. |

The kill is the most valuable outcome. A kill with evidence saves months. A kill without evidence is just stopping.

---

## Bet Size Distribution

This is what a healthy portfolio looks like. The distribution shifts as the team matures — early teams skew heavily toward Scouts, experienced teams hold a balanced portfolio.

| Bet Size | Target Distribution | Duration | When to Use |
|---|---|---|---|
| **Scout** | 40–50% | Hours to 2 days | Low confidence. "We think this might matter." One signal, one experiment. |
| **Sprint** | 30–35% | 1–2 weeks | Medium confidence. "Evidence suggests this." Validated in a Scout or prior cycle. |
| **Campaign** | 15–20% | 2–4 weeks | High confidence. "Validated in Scout/Sprint." Cross-functional execution required. |
| **Moonshot** | 0–5% | 4–8 weeks | Very high confidence. "Strategic commitment." Only after multiple validation cycles. |

**Red flags:**
- More than 30% Campaigns with no Scouts feeding them — the team is skipping validation.
- Zero Moonshots across four quarters — the team is playing it too safe. No structural bets.
- More than 60% Scouts after Q2 — the team is learning but not committing. Signal without action.

---

## Time Per LEAP Stage

First-cycle teams move slower because the system is new. By Q3, the AI's compound context cuts cycle time dramatically.

| Stage | First Cycle | Experienced Team | What Drives the Difference |
|---|---|---|---|
| **LEARN** (Strategy + Opportunity Map) | 3–5 days | 1–2 days | AI synthesizes prior evidence. TAP scoring reuses validated data from previous cycles. |
| **EXPLORE** (Brief + Prototypes + Pre-mortem) | 5–7 days | 1–3 days | Parallel-synthesis agents produce multi-perspective briefs in minutes. Prototypes generate from briefs in hours. |
| **ACTION** (Bet Card + Execution) | Varies by bet size | Varies by bet size | Bet card generation drops from hours to minutes. The interview agent auto-resolves from context vault. |
| **PROVE** (Evidence + Decision) | 2–3 days | Same day to 1 day | Evidence templates pre-populated by AI. Decision routing is immediate. |
| **Full Scout cycle** | 3–5 days | 1–2 days | The target. A Scout should resolve within a week, even on the first cycle. |
| **Full Sprint cycle** | 2–3 weeks | 1–2 weeks | Includes execution time. LEAP compresses everything except the actual building. |

If LEARN takes more than a week, the team is over-researching before ranking. Rank first, then go deep.

---

## TAP Scoring Guide

TAP — Total Addressable Pain. Reach × Frequency × Intensity. The score determines what happens next.

| TAP Score | Action | What It Means |
|---|---|---|
| **8–10** | Prioritize immediately | High reach, high frequency, high intensity. This is a burning problem for a large segment. Move to EXPLORE now. |
| **5–7** | Sprint bet | Meaningful pain but scoped. Worth a 1–2 week Sprint to validate the solution approach. |
| **3–4** | Park | Real but low urgency. Log it. The AI will surface it again if evidence accumulates. |
| **1–2** | Don't invest | Low reach, low frequency, or low intensity. Not worth a Scout. The opportunity cost is too high. |

**Scoring dimensions:**

| Dimension | 1 (Low) | 2 | 3 (High) |
|---|---|---|---|
| **Reach** | <10% of segment | 10–40% of segment | >40% of segment |
| **Frequency** | Rare (quarterly or less) | Regular (weekly/monthly) | Daily or near-daily |
| **Intensity** | Notice (minor friction) | Frustrate (workaround needed) | Abandon (customer leaves or switches) |

Multiply, don't average. A daily problem that causes abandonment for 50% of users is a 27. A quarterly annoyance for 5% is a 1. TAP makes the gap obvious.

---

## Customer Relationship Hierarchy — Indicators Per Stage

Solve the current stage before building for the next. This is Maslow for product.

| Stage | The Customer Says | Key Indicators | What to Build |
|---|---|---|---|
| **Functional** | "It doesn't work" / "I can't find what I need" | High error rates. Core flows broken. Support tickets on basic functionality. Task completion <70%. | Fix the fundamentals. Search, navigation, core transaction flow. No features until the floor is solid. |
| **Trustworthy** | "I can't rely on it" / "It works sometimes" | Inconsistent delivery/performance. NPS detractors cite reliability. Repeat usage declining despite acquisition. | Consistency, reliability, accuracy. Promise what you deliver. Deliver what you promise. |
| **Engaging** | "It's fine but nothing special" | Flat retention curves. Low feature adoption. Customers use 1–2 features only. No organic referrals. | Reduce friction. Surface value the customer is not discovering. Make the experience worth choosing over alternatives. |
| **Valuable** | "I'd miss it if it were gone" | Healthy retention. Expanding usage (new features, higher frequency). Willingness to pay or upgrade. | Deepen the relationship. Personalization. Cross-sell. Make the product more useful the more they use it. |
| **Loved** | "I tell people about it" | Organic referrals. High NPS promoters. Community engagement. Brand affinity beyond the transaction. | Invest in advocacy. Community. Identity. The product becomes part of how the customer sees themselves. |

**The diagnostic:** If your roadmap has Valuable-stage features and your metrics show Functional-stage problems, you have a Relationship Stage Mismatch. Stop building delight. Fix the floor.

---

## Quality Gate Thresholds

Every artifact generated in LEAP is scored 0–100 by the AI quality reviewer before it enters the tree. The score determines what happens next.

| Score | Action | What It Means |
|---|---|---|
| **70–100** | **Publish** | Meets quality standards. Published to the tree. PM reviews and decides. |
| **50–69** | **Watch** | Partially formed. Parked in a watchlist. The AI provides specific feedback on what's missing. Regenerate or manually improve. |
| **Below 50** | **Park** | Not ready. Logged for context but not surfaced in active workflows. Common for first-pass opportunity candidates with insufficient evidence. |

**What the score measures:**
- Completeness — are all required fields populated with substance, not filler?
- Evidence quality — are claims sourced or assumed?
- Internal consistency — does the hypothesis match the measurement plan? Do kill criteria align with the bet size?
- Context alignment — does the artifact connect to the parent node's strategy and opportunity?

A team averaging below 60 on first-pass artifacts is under-investing in LEARN. The AI generates better outputs when the context tree is richer. Low scores are a symptom of thin context, not poor AI performance.

---

## 90-Day Adoption Milestones

What a team should achieve in the first 90 days of running LEAP. These are not aspirational — they are the minimum indicators that the system is taking hold.

| Day | Milestone | Why It Matters |
|---|---|---|
| **Day 7** | First Scout bet resolved | Proves the team can write a hypothesis, run a small experiment, and make a ship/iterate/pivot/kill decision. The system sells itself after the first kill. |
| **Day 14** | Opportunity map with 5+ TAP-scored opportunities | LEARN is operational. The team is ranking before researching. Comparison, not conviction, is driving prioritization. |
| **Day 30** | 3+ bets resolved (mix of Scout and Sprint) | The rhythm is forming. Evidence is starting to compound. The tree has enough nodes for the AI to synthesize meaningfully. |
| **Day 45** | First kill with full evidence archive | The team has demonstrated the hardest behavior: stopping something that is not working and preserving the learning. This is the cultural inflection point. |
| **Day 60** | Second-generation bet (a bet informed by a previous bet's evidence) | Compound context is working. The team is not starting from scratch. Each cycle is smarter than the last. |
| **Day 75** | Strategy.md updated based on accumulated evidence | PROVE is flowing upward. Evidence from resolved bets is changing the strategy, not just validating it. The tree is alive. |
| **Day 90** | 8–12 bets resolved. Kill rate 25–40%. At least one Pivot. | The system is running. The team is learning faster than they are building. The compound flywheel has its first rotation. |

If Day 30 passes without a resolved bet, the team is treating LEAP as a planning tool, not a discovery system. Intervene.

---

## The Compound Effect — Why These Numbers Matter

These benchmarks are not performance targets to be gamed. They are diagnostic signals.

A team hitting these numbers is learning at a rate that makes their competition structurally slower. More resolved bets produce more evidence. More evidence produces better-informed future bets. Better-informed bets resolve faster. Faster resolution produces more resolved bets. The flywheel compounds.

A team missing these numbers is not "behind." They are running a different system — likely a traditional roadmap with LEAP vocabulary bolted on. The fix is not to work harder. The fix is to resolve one Scout bet by Friday.

---

*Build less. Learn more. Let the AI execute. You decide.*

---

*Tony Fadel · CPO · 20+ years in product · Building from the UAE · Software has no soil conditions.*

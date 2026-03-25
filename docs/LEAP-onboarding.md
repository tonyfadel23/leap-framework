# How to Roll Out LEAP
## A 90-day playbook for product managers and engineers

---

## The wrong way to introduce LEAP

Don't present it as a process change. Don't send a 40-page doc. Don't schedule a "framework alignment workshop." Don't create a Confluence page.

These all fail for the same reason: they position LEAP as overhead. One more thing on top of delivery.

LEAP is not an addition. It's a replacement of the mental model. "Ship features, measure output" becomes "resolve bets, measure learning." That replacement cannot be taught in a presentation. It has to be experienced in a cycle.

---

## Week 0: Pick the pilot team

One product trio: PM + Designer + Engineer. Not the most experienced team. Not the one with the most bandwidth. Pick the team with the most painful open question — the one where nobody knows what to build next.

That pain is the seed. LEAP doesn't need converts. It needs a problem worth solving.

---

## Week 1-2: The first cycle (10 days)

### Days 1-2: LEARN

Pick one goal. Write it as a metric: baseline → target → deadline. Not "improve retention" — "increase 7-day retention from 22% to 30% by end of Q3."

Map three opportunities. Not features. Problems. Use JTBD format: "When [trigger], I want to [job], so I can [outcome]." Score each by TAP. Filter by Customer Relationship Hierarchy.

**The engineer's role:** Engineers see systems, not surfaces. They spot structural constraints PMs miss. "We can't personalize because the data model doesn't support preferences" — that's an opportunity the PM would never find in interviews.

### Days 3-5: EXPLORE

Generate three solutions. Not one. Three. Each materially different. PM brings the framing. Designer sketches the experience. Engineer flags feasibility.

Pre-mortem each in 30 minutes: "It's six months from now and this failed. Why?" Tigers (real threats), Paper Tigers (false fears), Elephants (nobody's saying it).

Build a prototype of the strongest one. With AI: two hours, not two weeks. Show it to three users.

**The engineer's role:** Prototype feasibility. "Can we actually query this in real-time?" matters more than pixel-perfect design at this stage.

### Days 6-8: ACTION

Turn the winner into a bet card. Hypothesis, execution plan, measurement, prove criteria. Pick a bet size:

- **Scout** (hours): cheapest test for one signal
- **Sprint** (1-2 weeks): validated mechanism
- **Campaign** (2-4 weeks): scaled confidence
- **Moonshot** (4-8 weeks): strategic commitment

The engineer builds. The PM instruments measurement. The bet card's prove criteria are the contract.

### Days 9-10: PROVE

Look at the data. Make the call: ship, iterate, pivot, or kill.

If the call is "kill" — celebrate it. A kill with evidence is worth more than a ship without it. The kill just saved months.

Route the decision. Document the learning. Close the cycle.

---

## Week 3: The retro

60 minutes. Three questions:

1. **What did we learn that we wouldn't have learned the old way?**
2. **Where did the framework feel like overhead vs. where did it feel like clarity?**
3. **What would we change for the next cycle?**

The answer to question 1 sells LEAP to the rest of the org. Document it. Share it.

---

## Week 4-6: Expand to two more teams

Don't mandate. Invite. Share the pilot team's findings. Let the results speak.

90-minute kickoff for each new team:
- **30 min:** Pilot team tells their story — what they learned, what they killed, what they shipped
- **30 min:** Framework walkthrough — L→E→A→P, tree structure, bet sizing, prove criteria
- **30 min:** Each team picks their goal and maps first opportunities

Then they run their own 10-day cycle. The pilot PM coaches.

---

## Month 2: The org-level shift

Three teams running LEAP with results. The shift happens when you change what leadership reviews.

**Stop reviewing:** Feature roadmaps. Story points. Sprint velocity.

**Start reviewing:** Bets resolved per team per quarter. Evidence quality. Kill rate.

A healthy kill rate is 30-40%. It means you're testing real hypotheses, not confirming what you already believe.

The quarterly review becomes: "Show me your tree. Where did you start? What did you learn? What did you kill? What compounds?"

---

## The engineer onboarding track

Engineers need three concepts, not the full framework:

### 1. The node tree
"Every piece of work lives in a tree. Your code maps to an ACTION node. That ACTION lives under an EXPLORE concept, under a LEARN opportunity. When you write code, you know which hypothesis it tests."

### 2. The bet card
"Before you build, there's a bet card. It tells you what we're testing, how we'll measure it, and when to stop."

### 3. The kill criteria
"Every bet has kill criteria defined before you start. If the data hits them, we stop. No sunk cost arguments."

Engineers who understand these three concepts ask the PM: "What's the prove criteria for this ticket?" That question alone changes the quality of every standup.

---

## The PM onboarding track

Three skills to practice:

### 1. Opportunity mapping (LEARN)
Take your current roadmap. For every feature, ask: "What customer problem does this solve?" Rewrite each as an opportunity in JTBD format. Score by TAP. Half your roadmap is solutions looking for problems.

### 2. Pre-mortem thinking (EXPLORE)
Take your favorite idea. Assume it failed. Write three reasons why. Ask: "Which failures would we only discover after building?" That's your riskiest assumption. Test it first.

### 3. Pre-commitment (ACTION)
Before any work starts, write prove criteria: "Ship if X. Iterate if Y. Pivot if Z. Kill if W." Pin it to the wall. Reference it every standup.

---

## The mutation mechanism

John Cutler is right: frameworks calcify. LEAP avoids this with a built-in feedback loop.

Every resolved bet generates evidence. Evidence updates the opportunity map. The opportunity map reshapes strategy. Strategy reframes the next cycle's LEARN phase.

The framework doesn't stay static. It evolves with every cycle because the tree it operates on evolves. No two cycles look the same — because the accumulated evidence changes what's possible.

If your LEAP tree looks the same after three cycles as it did after one, you're not running LEAP. You're following a checklist.

---

## Who is accountable?

Marty Cagan's question is the right one: when AI generates and the PM decides, who owns the outcome?

The PM. Always.

- **Value risk** — the PM owns it. "Will customers use this?" is a human judgment call.
- **Usability risk** — the designer owns it. AI prototypes, humans validate.
- **Feasibility risk** — the engineer owns it. AI estimates, humans verify.
- **Viability risk** — the PM owns it. Business context is human context.

AI makes the evidence richer. The human still makes the call. Accountability doesn't diffuse because the execution automated. It concentrates because the decisions matter more.

---

## Anti-patterns to watch

**"We do LEAP but still have a feature roadmap."** The tree IS the roadmap. No tree, no LEAP.

**"We ran LEARN but skipped EXPLORE."** You jumped to the first idea. The whole point of EXPLORE is to prevent that.

**"We don't kill anything."** Kill rate 0% = you're not testing real hypotheses.

**"PROVE happens at the end."** PROVE is a layer, not a phase. If you only evaluate at the end, you're doing waterfall with extra steps.

**"The engineers don't know about the bet."** Every engineer should answer: "What hypothesis does my work test?" If they can't, the PM hasn't done their job.

---

## 90-day calendar

| Week | Action | Who |
|------|--------|-----|
| 0 | Pick pilot team | Leadership |
| 1-2 | First LEAP cycle | 1 trio + coach |
| 3 | Retro + document learnings | Pilot team |
| 4 | Invite 2 teams, 90-min kickoff | 3 trios |
| 5-6 | Teams 2-3 run first cycle | 3 trios |
| 7 | Cross-team retro | All trios |
| 8 | Leadership review: bets, not features | Leadership |
| 9-10 | Open enrollment | Org-wide |
| 11-12 | First quarterly review with LEAP metrics | Leadership |

---

## What success looks like at 90 days

- 3+ teams running LEAP independently
- At least one celebrated kill
- Leadership asking "what bets did you resolve?" instead of "what did you ship?"
- Engineers asking "what's the prove criteria?" in standups
- An opportunity tree updated 4+ times
- The phrase "bets resolved per quarter" in at least one leadership review

The framework doesn't need evangelism after 90 days. The results evangelize themselves.

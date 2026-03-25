# Stop Measuring Features Shipped. Start Measuring Bets Resolved.

*Something I understood too late: the teams I led that shipped the most features were not my best teams. They were my most expensive failures.*

---

## This Is Not a Discovery Problem. It's a Decision Architecture Problem.

Product teams don't have a discovery problem. They have a decision problem.

Every PM I've worked with in twenty years can find opportunities. They can talk to customers, read dashboards, map pain points. Discovery is not the bottleneck. The bottleneck is what happens after discovery: the decision to build, the absence of kill criteria, the inability to stop, the organization's gravitational pull toward shipping something — anything — to justify the quarter.

The product roadmap is a graveyard of unvalidated assumptions dressed up as commitments. A team ships forty features in a quarter and calls it velocity. But velocity without signal is just expensive movement. You're running fast. You have no idea if you're running in the right direction. And by the time you find out, you've spent six months and three engineers on something no one needed.

I spent two decades watching this happen. I spent the last year building the alternative.

It's called LEAP — Learn, Explore, Action, Prove. And the unit of progress is not the feature shipped. It's the bet resolved.

---

## The Feature Factory Has Better Tools Now. It's Still a Feature Factory.

Every product tool on the market does the same thing: takes the existing PM workflow and adds AI. Write a PRD faster. Summarize user interviews. Auto-generate acceptance criteria. AI as autocomplete for the same broken process.

A faster car on the same road does not change where the road goes.

Write a PRD in ten minutes instead of three hours. Great. You still wrote one PRD for one solution. You still didn't test the assumption. You still shipped without defining what failure looks like. The process is the problem — and making the process faster makes the problem worse, not better.

LEAP was not designed as a traditional framework that later got AI bolted on. It was designed from scratch as a system where AI is the execution layer and humans are the decision layer. Remove the AI and you don't get a simpler framework. You get nothing. Like removing the engine from a car — it's not a slower car, it's a sculpture.

The framework and the AI are architecturally inseparable. Twenty years of product experience designed the decision architecture. AI designed the execution architecture. LEAP is what happens when both are built at the same time, for the same system, from the ground up.

---

## A Decision That Went Wrong — And What It Taught Me

A team once pitched me a beautiful recommendation engine. Personalized suggestions, machine learning, the works. They had the competitive analysis, the user research, a prototype that looked sharp. The pitch was tight.

I asked one question: "What relationship stage are we in with this segment?"

Functional. Customers couldn't find their last order. Search was broken. The basic promise — you can find what you want and trust it arrives — was not met.

The Customer Relationship Hierarchy killed the project in one question. You don't build personalization when search is broken. You don't build delight when customers can't trust your delivery time. Maslow applies to product: solve the current stage before building for the next.

That team had spent three months on a recommendation engine that addressed the wrong level of the hierarchy. Three months, four engineers, a designer, a data scientist. All producing something customers didn't need yet — because the team never asked what the customer needed first. They started with the solution and worked backwards to justify it.

This is the disease. And faster PRD writing doesn't cure it.

---

## How LEAP Actually Works: Three Stages, One Layer

LEAP has three stages — **Learn**, **Explore**, **Action** — and one continuous evaluation layer: **Prove**.

The stages are sequential in concept, fluid in practice. Prove is not a phase. It runs across all three, constantly asking: *Based on what we now know, should we continue, change direction, or stop?*

### Learn: The Problem Is Not "What Should We Build?"

The problem is: what problem is worth solving, for whom, and why now?

Most teams skip this. They start with a solution and work backwards to justify it. Or they do "discovery" — which means talking to five users about a feature they've already decided to build.

LEARN forces ranking before research. Every opportunity is scored using your chosen rationalisation framework — Total Addressable Pain:

**TAP = Reach x Frequency x Intensity**

TAP, not TAM. Pain drives behavior change. Revenue projections don't. A problem affecting 80% of your users daily at high intensity is worth more than a problem affecting 5% of users monthly at low annoyance — regardless of the revenue model attached to either.

Then the Customer Relationship Hierarchy filters what gets worked on next: Functional, Trustworthy, Engaging, Valuable, Loved. This is Maslow for product. Solve the current stage before building for the next.

Three AI agents analyze the same problem space in parallel — Strategist (market lens), Researcher (user lens), Analyst (systems lens). A synthesis agent merges their perspectives. The PM gets a multi-perspective strategy document in minutes that would take a cross-functional team days. The PM's job: critique it, challenge the scoring, decide which opportunity to pursue.

### Explore: Generate Alternatives, Not Confirmations

Not one solution — multiple. At least three. Each materially different enough to test a different assumption.

The engine: Diverge, Stress-Test, Converge.

Stress-Test runs a pre-mortem on each option: "It's six months from now and this solution failed. What happened?" Classify the risks. Tigers — real threats that will kill you. Paper Tigers — fears that dissolve on inspection. Elephants — obvious problems nobody is naming.

Two years ago, a prototype took two weeks. Now it takes two hours. You generate five interactive prototypes in a morning and show them to users by lunch. This workflow is impossible without AI. EXPLORE went from bottleneck to accelerator.

### Action: Place the Bet, Define the Kill Criteria

Every solution becomes a bet. Every bet has a size:

- **Scout** — hours to two days. Low confidence. "We think this might matter."
- **Sprint** — one to two weeks. Medium confidence. "Evidence suggests this."
- **Campaign** — two to four weeks. High confidence. "Validated in Scout/Sprint."
- **Moonshot** — four to eight weeks. Very high confidence. "Strategic commitment."

The size matches your confidence. Low confidence does not get a Campaign. It gets a Scout — four hours, one signal.

The bet card defines four things before execution starts: the hypothesis, the execution plan, the measurement criteria, and the prove criteria — ship if A, iterate if B, pivot if C, kill if D.

This is pre-commitment. You are not deciding what to do with the results in the heat of the moment — surrounded by sunk cost bias and organizational pressure to ship. You decided before you started.

### Prove: The Kill Is the Most Valuable Outcome

When a bet resolves, the decision routes back through the system. Ship exits the loop. Iterate creates a new bet under the same concept. Pivot sends you to a new concept under the same opportunity. Kill archives with evidence.

A kill with evidence saves months of building the wrong thing. The kill rationale becomes organizational memory. Six months later, someone has the same idea, opens the tree, and finds: "We tested this. Here's what happened. Here's why we stopped."

Teams that celebrate kills learn faster than teams that only celebrate launches.

---

## The Compound Effect Is the Moat

After three quarters of running LEAP, something structural changes. The system compounds.

Quarter one: five bets resolved. Mostly Scouts. The team is learning the system. Quarter two: twelve bets resolved. Each bet starts with Q1's evidence. Kill decisions take days, not weeks. Quarter three: eighteen or more bets resolved. New bets inherit fifty previous evidence artifacts. The AI reads all of it before generating anything new.

More resolved bets produce more evidence, which produces better-informed future bets, which resolve faster, which produces more resolved bets. This is a compounding data flywheel.

The tenth bet in a workspace is structurally smarter than the first because it stands on the shoulders of nine previous cycles. Traditional PM tools don't compound. Each PRD starts from a blank page. Each research project starts from scratch. LEAP was designed so that the system gets better at your specific product with every cycle.

The metric that matters: bets resolved per quarter. Not features shipped. A team resolving fifteen bets with evidence will outperform a team shipping fifty features without signal. Every single time.

---

## The PM Decides. AI Executes.

I want to address the accountability question directly, because it's the right question.

Marty Cagan's four risks — value, usability, feasibility, viability — still need a human accountable for each one. LEAP does not change this. When AI generates and the PM decides, the PM owns the outcome. Full stop.

The PM sets the goal. Critiques the strategy. Challenges the opportunity scoring. Picks the bet size. Defines the kill criteria. Makes the ship/iterate/pivot/kill call.

Everything between those decisions — research synthesis, brief generation, prototype creation, quality scoring, evidence compilation — is executed by AI.

This is not a diminishment of the PM role. It's an elevation. The PM stops being a writer of documents and becomes a judge of decisions. The thinking gets harder, not easier. The decisions get better because the evidence is richer.

Less writer. More editor. Less producer. More judge.

---

## What This Is NOT

**Not a replacement for customer empathy.** AI accelerates execution. It does not replace the judgment that comes from sitting with a customer and watching them struggle. Signal before scale applies to understanding, not just shipping.

**Not a process you follow mechanically.** The moment you run LEAP as a checklist without engaging your judgment, you've built a feature factory with better labels. The framework demands that the PM thinks at every decision point. If you're not challenging the AI's scoring, you're not using LEAP — you're outsourcing your judgment.

**Not a linear process.** L-E-A looks sequential. In practice, Prove sends you back constantly. A killed bet sends you to Learn. A pivoted concept sends you to Explore. The tree is the system of record, not a Gantt chart.

**Not a way to skip the hard conversations.** Organizational politics, stakeholder alignment, the executive who wants their pet feature on the roadmap — LEAP doesn't make those disappear. What it does is give you evidence. When someone asks "why didn't you build X?" you open the tree and show them: "We tested it. Here's the hypothesis. Here's the result. Here's why we killed it." Evidence is the best defense against opinion.

---

## What to Do Monday Morning

You don't need LEAP software to start. You need the discipline.

1. **Pick one goal.** Write it as a metric with a baseline and a target. Not "improve retention." Instead: "Move 30-day retention from 42% to 50%."

2. **Map three opportunities and score them.** Score each by reach, frequency, and intensity. Pick the highest-pain one. Not the most interesting one. Not the one with the best revenue model. The one with the most pain.

3. **Generate three materially different solutions.** Pre-mortem each in thirty minutes. Name the Tigers, the Paper Tigers, and the Elephants.

4. **Build a Scout bet.** Define the hypothesis: "If we do X, metric Y moves by Z." Define the kill criteria before you start. Write it down. Share it with the team.

5. **Resolve it by Friday.** Ship, iterate, pivot, or kill. Record the evidence. Share the outcome.

The system sells itself after the first kill. That's when the team realizes they saved three months of building the wrong thing. And they have the evidence to prove it.

---

## The Vision, Specific Enough to Test

Here is what I believe product management looks like in three years.

The best product teams will resolve thirty or more bets per quarter. They will have organizational memory spanning hundreds of evidence artifacts. A new PM joining the team will open the tree and understand — in an afternoon — every assumption tested, every hypothesis validated or killed, every pivot rationale, every competitive signal that changed direction.

Features shipped will not appear on any performance review. Bets resolved — and the quality of the decisions those bets produced — will be the measure.

The PM who writes the best PRDs will be less valuable than the PM who makes the best ship/kill decisions. The PM who ships the most will be less valuable than the PM who kills the fastest with the least waste.

The product roadmap — the artifact that has governed product management for twenty years — will be replaced by the evidence tree. Not because roadmaps are evil, but because they encode commitments before evidence exists. The evidence tree encodes learning. And learning compounds.

I believe this shift is structural, not incremental. The teams that make it will build defensible products. The teams that don't will keep shipping features into the void and wondering why nothing moves.

Build less. Learn more. Let the AI execute. You decide.

---

*Tony Fadel. CPO. 20+ years in product. Building from the UAE. Software has no soil conditions.*

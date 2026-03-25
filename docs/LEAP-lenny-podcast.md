# Lenny's Podcast: LEAP — The AI-First Product Discovery System
## A Conversation with Tony Fadel

---

**Lenny Rachitsky:** Tony, welcome to the podcast. You've been building product for twenty-plus years, you're running a 500-person product and tech org out of the UAE, and you've built something called LEAP that I think is going to challenge how a lot of people in this audience think about discovery. Give us the one-sentence version.

**Tony Fadel:** LEAP is a system where AI runs the entire discovery loop and the PM's only job is to decide: ship, iterate, pivot, or kill.

**Lenny:** That's going to make some people uncomfortable. Let's get into it. Before we talk about the framework itself — what's the problem you kept seeing over twenty years that made you build this?

**Tony:** The product roadmap is a graveyard of unvalidated assumptions. That's the problem. I've watched hundreds of teams ship confidently and learn nothing. They run a sprint, they ship a feature, they move to the next ticket. Nobody asks: did this work? And if it didn't work, nobody asks: why not?

The unit of progress in most product teams is the feature. Or the story point. Or the release. None of those are learning. A team can ship fifty features in a quarter and have zero signal about whether any of them mattered. I've seen it. Repeatedly.

**Lenny:** So the issue isn't that teams aren't shipping — it's that they're shipping without learning.

**Tony:** Exactly. Shipping is not the bottleneck. Signal is the bottleneck. The question is not "how fast can we build?" The question is "how fast can we learn whether we should have built it at all?" And most teams never answer that question. They just move to the next feature.

**Lenny:** OK, so LEAP is your answer to this. Walk us through it.

**Tony:** Three stages, one layer. LEARN, EXPLORE, ACTION — those are the stages. PROVE is not a stage. It's a continuous evaluation layer that runs across all three. At every point in the loop, PROVE asks: based on what we now know, should we continue, change direction, or stop?

**Lenny:** Let's take them one at a time. LEARN.

**Tony:** LEARN is where most teams skip. They start with a solution and work backwards to justify it. Or they do what they call "discovery" — which usually means talking to five users about a feature they've already decided to build. That's not discovery. That's confirmation.

LEARN forces you to answer the real question: what problem is worth solving, for whom, and why now? Not what should we build. What pain is big enough to justify the investment?

Every opportunity in LEARN is scored by what I call TAP — Total Addressable Pain. Not TAM. TAM tells you the revenue ceiling. TAP tells you whether anyone will change their behavior.

**Lenny:** Break down TAP for me.

**Tony:** Three variables. Reach — what percentage of the segment is affected. Frequency — is this a daily pain, weekly, monthly, or rare? And Intensity — does the user abandon, get frustrated, get annoyed, or barely notice?

Reach times Frequency times Intensity. That's TAP. A problem that affects 80% of users daily and causes abandonment is a different animal than a problem that affects 5% of users once a month and mildly annoys them. TAP separates the two instantly.

**Lenny:** I love that. It's like NPS but for the problem, not the product.

**Tony:** And then there's a second filter — the Customer Relationship Hierarchy. Think of it as Maslow for product. Five stages: Functional, Trustworthy, Engaging, Valuable, Loved. You don't build personalization when search is broken. You don't build delight when customers can't trust your delivery time. Solve the current stage before building for the next.

**Lenny:** Can you give us a concrete example of that in practice?

**Tony:** A team once pitched me a beautiful recommendation engine. Gorgeous UX. Smart algorithm. They were excited. I asked one question: "What relationship stage are we in with this segment?" The answer was Functional. Customers in that segment couldn't find their last order. They were struggling with basic navigation.

The Relationship Hierarchy killed the project in one question. You don't build a recommendation engine for a customer who can't find the search bar. That's LEARN doing its job. And by the way — that kill saved us months of engineering time on something that would have failed, because the foundation wasn't there.

**Lenny:** That's the kill story. And you think the kill is actually the most valuable outcome.

**Tony:** The kill is the most valuable outcome. Full stop. A kill with evidence saves months of building the wrong thing. Every team I've worked with — the moment they experience their first evidence-backed kill, they become believers. Because they realize: we were about to spend a quarter on that. And we have the evidence to prove it would have failed.

But it's more than that. The kill rationale becomes organizational memory. Six months later, someone has the same idea. They open the tree, and they find: we tested this. Here's what happened. Here's why we stopped. That's compound learning. The organization gets smarter, not just the individual.

**Lenny:** OK let's keep going. EXPLORE.

**Tony:** EXPLORE is where you generate alternatives. Not one solution — multiple. At least three. Each materially different enough to test a different assumption.

The engine is three steps: Diverge, Stress-Test, Converge. Diverge generates options. Stress-Test runs a pre-mortem on each — "It's six months from now and this solution failed. What happened?" You classify the risks. Tigers — real threats. Paper Tigers — fears that dissolve on inspection. Elephants — obvious problems nobody is naming. Converge picks the approach with the best risk-to-signal ratio.

**Lenny:** I like the Tiger taxonomy. Where does that come from?

**Tony:** It's a framework I built after watching teams either over-index on risks that don't matter or completely ignore the one that's sitting in the middle of the room. Paper Tigers eat weeks of meeting time. Elephants eat products. You need to know which one you're looking at.

**Lenny:** And then ACTION.

**Tony:** Every solution becomes a bet. Every bet has a size. Scout — hours to two days, low confidence, "we think this might matter." Sprint — one to two weeks, medium confidence, "evidence suggests this." Campaign — two to four weeks, high confidence, "validated in a Scout or Sprint." Moonshot — four to eight weeks, very high confidence, strategic commitment.

The size matches your confidence. Low confidence does not get a Campaign. It gets a Scout. Four hours, one signal. This is where most teams get it wrong — they have a hunch and immediately allocate a two-week sprint to it. That's over-investment. Run a Scout. Get a signal. Then decide whether it deserves the Sprint.

**Lenny:** And the bet card — what goes on it?

**Tony:** Four things, all defined before execution starts. Hypothesis: if we do X, then metric Y will move by Z. Execution plan: who builds what, by when. Measurement: primary metric, counter-metrics, duration. And Prove criteria: ship if A, iterate if B, pivot if C, kill if D.

This is pre-commitment. You are not deciding what to do with the results in the heat of the moment — surrounded by sunk cost bias and organizational pressure to ship. You decided before you started. That's the whole point. The bet card is a contract with your future self.

**Lenny:** That's powerful. Let me push back on something, though. How is this different from Teresa Torres' Opportunity Solution Tree? Because there's clearly overlap — opportunity mapping, continuous discovery, the tree structure.

**Tony:** Teresa Torres is the genealogy. LEAP is the operating system.

Let me unpack that. OST gave us the right mental model — opportunity trees, not feature lists. Continuous discovery, not discovery phases. That insight is foundational. I cite Torres regularly. LEAP inherits those concepts.

But OST is a thinking framework. It tells you how to organize your thinking. LEAP is an execution system. It tells the AI how to run. There are agents, quality gates, parallel synthesis, auto-generated prototypes, compound context that persists across cycles. OST doesn't have bet sizing. It doesn't have TAP scoring. It doesn't have kill criteria pre-committed on a bet card. It doesn't have a Prove layer that continuously evaluates whether to continue or stop.

Think of it this way. If Torres gave us the map, LEAP gives you the vehicle, the fuel, and the navigation system. And the vehicle happens to be self-driving. The PM sets the destination and makes the judgment calls. The AI drives.

**Lenny:** That's a clean distinction. Let's talk about the AI piece, because I think that's where this gets really different. You say LEAP is AI-first, not AI-augmented. What does that mean in practice?

**Tony:** Every product tool on the market is doing the same thing: taking the existing PM workflow and adding AI to it. Write a PRD faster. Summarize user interviews. Auto-generate acceptance criteria. AI as autocomplete for the same broken process.

This is not what LEAP does. LEAP was designed from scratch assuming AI exists. Not adapted. Designed. Remove the AI and you don't get a simpler framework. You get nothing. Like removing the engine from a car — it's not a slower car, it's a sculpture.

**Lenny:** Give me the specific things AI does in LEAP that couldn't happen in a traditional workflow.

**Tony:** Five things. First — context synthesis is instant. The AI reads your org strategy, your business line context, your workspace research, your node documents. It builds a complete contextual picture in seconds. A PM doing this manually spends a day reading Confluence.

Second — multiple perspectives are parallel, not sequential. In LEARN, three AI agents analyze the same problem space simultaneously. Strategist looks at market dynamics. Researcher looks at user evidence. Analyst looks at systems impact. A synthesis agent merges them. That's not "faster analysis." That's a fundamentally different analytical architecture.

Third — prototyping is a thinking tool, not a deliverable. LEAP generates interactive prototypes from product briefs. Not wireframes. Working HTML. Two years ago, a prototype took two weeks. Now it takes two hours. You generate five prototypes in a morning and show them to users by lunch. That workflow is impossible without AI.

Fourth — quality gates are continuous. Every document generated by LEAP is scored by an AI quality reviewer before it's published. Below 70 out of 100, it gets regenerated with specific feedback. The system assumes every output will be machine-generated and therefore needs machine-checked quality.

Fifth — compound context. Every cycle enriches the tree. Every resolved bet adds evidence. Every kill adds a rationale. The AI reads all of it before generating anything new. The tenth bet in a workspace is smarter than the first because it stands on nine previous cycles.

**Lenny:** That fifth one is huge. You're basically saying the system gets smarter at your specific product over time.

**Tony:** That's exactly what I'm saying. Traditional PM tools don't compound. Each PRD starts from a blank page. Each research project starts from scratch. LEAP was designed so that the AI gets better at your specific product, your specific customers, your specific competitive landscape — with every cycle.

I use the analogy of a horse carriage versus an automobile. You can put a motor on a horse carriage. That's augmentation. Or you can design a vehicle from scratch that assumes the motor exists. The frame is different. The wheels are different. The steering is different. Everything is different because it was designed for the engine. That's what LEAP does with AI.

**Lenny:** Let me ask the question I think a lot of listeners are thinking right now. This sounds amazing for a team with the resources to do weekly continuous discovery. But what about a team of three PMs, moving fast, who can barely find time for user interviews? Can they actually use LEAP?

**Tony:** LEAP scales down to Scout bets. That's the whole point of bet sizing.

A Scout is hours to two days. One hypothesis, one signal. You don't need a dedicated research team. You don't need a two-week sprint. You need one goal, one opportunity scored using your chosen rationalisation framework, one hypothesis, and one kill criteria. That's it.

Monday morning. Pick one goal. Write it as a metric with a baseline and a target. Map three opportunities and score them — pick the highest-pain one. Generate three solutions, pre-mortem each in thirty minutes. Build a Scout bet. Define the hypothesis and the kill criteria. Resolve it by Friday.

A team of three PMs can do that. A solo PM can do that. The AI handles the synthesis, the prototype generation, the quality scoring. The PM makes the calls. The bet card takes ten minutes to generate. The Scout resolves in a day or two. That's LEAP at minimum viable scale.

**Lenny:** So it's not an all-or-nothing framework.

**Tony:** It's designed to be entered at any altitude. Run Scouts for a quarter. Get comfortable with pre-committed kill criteria. Start resolving bets. Then graduate to Sprints when the evidence warrants it. The system sells itself after the first kill. That's when the team realizes they saved three months of building the wrong thing.

**Lenny:** Let's talk about the compound effect over time. You have data on this?

**Tony:** Here's what we see. Quarter one: a team resolves roughly five bets. They're learning the system. Mostly Scouts. That's fine. Quarter two: they resolve twelve. Each bet starts with Q1's evidence. Kill decisions take days, not weeks, because the tree has context.

Quarter three: eighteen or more resolved bets. The compound flywheel is spinning. New bets inherit fifty-plus previous evidence artifacts. The AI is operating on a rich contextual base. Decisions get faster and more accurate simultaneously.

The metric that matters is bets resolved per quarter. Not features shipped. A team resolving fifteen bets with evidence will outperform a team shipping fifty features without signal. Every single time. It's like Manchester City under Guardiola — the passes per goal metric doesn't matter if the passes don't create chances. Features without signal are passes into empty space.

**Lenny:** I love that analogy. Let me ask one more thing before we go to the lightning round. You mentioned the PM's role changes. Some PMs are going to hear "the AI does everything between decisions" and feel threatened. What do you say to them?

**Tony:** The PM stops being a writer of documents and becomes a judge of decisions. That is not a diminishment. It's an elevation. The thinking gets harder, not easier. The decisions get better because the evidence is richer.

A PM who defines a sharp goal, challenges the TAP scoring, picks the right bet size, writes kill criteria that are honest, and makes a ship-or-kill call backed by evidence — that PM is more valuable than a PM who spends three days writing a PRD that nobody reads.

The craft shifts. Less writing, more judgment. Less producing, more critiquing. The PM who leans into that shift becomes more effective than they've ever been. The PM who clings to the old craft — "I write the PRD, I own the document" — they're defending a role that AI is going to subsume regardless. LEAP just makes it explicit.

**Lenny:** Direct. I appreciate that. Let's do the lightning round. Two or three books that have shaped your thinking.

**Tony:** *Empowered* by Marty Cagan — the foundational text on what a product team should be. *Continuous Discovery Habits* by Teresa Torres — the genealogy that LEAP builds on. And *7 Powers* by Hamilton Helmer — the best framework I've found for thinking about durable competitive advantage.

**Lenny:** Favorite product you're using right now that you think more people should know about.

**Tony:** Claude. And I know that sounds like a setup given this conversation, but I mean it structurally. What Anthropic built is the closest thing I've seen to a general-purpose reasoning partner. LEAP wouldn't exist without it. The multi-agent architecture, the parallel synthesis, the prototype generation — it all runs on the ability to have a reasoning engine that understands context at depth. That capability is genuinely new.

**Lenny:** Favorite interview question when you're hiring PMs.

**Tony:** "Tell me about a bet you killed and what evidence made you kill it." If they can't answer that, they've never done real discovery. They've shipped. They haven't learned.

**Lenny:** That's a strong filter. Last question — one contrarian opinion you hold about product management that most people would disagree with.

**Tony:** The best PMs will write almost nothing within five years. The craft of product management is not writing artifacts. It's making decisions under uncertainty. Every hour a PM spends writing a PRD is an hour they're not spending on judgment — challenging assumptions, stress-testing hypotheses, talking to customers. AI will write every artifact. The PM who thrives is the one who can judge what the AI produces and make the call. Less writer. More judge. Most of the industry is not ready to hear that.

**Lenny:** I think you're right that it makes people uncomfortable, and I also think you might be right. Tony, this has been great. What's the one thing you want people to take away?

**Tony:** Build less. Learn more. The resolved bet is the unit of progress — not the feature, not the sprint, not the story point. If you shipped it and you don't know whether it worked, you didn't make progress. You made inventory.

**Lenny:** Tony Fadel, thank you for being here. Where can people learn more about LEAP?

**Tony:** I'm building it in public. The framework docs are open. The thesis is simple — the product roadmap era is ending. The era of evidence-backed bets is starting. And it starts with one Scout bet, resolved by Friday.

**Lenny:** Build less, learn more. I dig it. Thanks, Tony.

**Tony:** Thanks, Lenny.

---

*Build less. Learn more. Let the AI execute. You decide.*

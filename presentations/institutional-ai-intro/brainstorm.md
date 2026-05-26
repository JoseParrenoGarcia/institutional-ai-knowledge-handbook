# Brainstorm — Institutional AI: The Discipline Presentation

> **Stage:** Initial brainstorm — flow and talking points, not final copy
> **Constraint:** ~15 minutes. Target 12–14 slides. No fluff.

---

## Narrative Arc

The talk needs a single emotional thread: *"Our work is about to compound in ways it never could before — but only if we change something small about how we think about knowledge."*

Open with a recognition moment (something they've all experienced). Define the concept with examples. Introduce the mechanisms — skills and hierarchical navigation. Show where we are and where we're going (maturity model). Build to a vision. Land on three things they can do next week.

---

## Section 1 — The Hook (1 min)

**Visual concept — two slides:**

**Slide 1A — "The Hunt"**
A caveman (cartoon vector, hunting pose) with three speech bubbles:
1. *"Why did we choose this model architecture and not the other one?"*
2. *"What do I actually need to know about this dataset before I start?"*
3. *"Has anyone in the discipline already solved something like this?"*

To the right: icons representing the hunt — Confluence, GitHub, a colleague (person icon). These are the prey.

**Slide 1B — "...eventually"**
Same caveman, defeated pose. One speech bubble:
> *"I found it. Three weeks later. I'd rather just be hungry."*

**Talking point (spoken over the two slides):**

> "Once upon a time, there was a data scientist looking for an answer. Not a hard answer — just context that someone, somewhere, had. So they hunted. Confluence. GitHub. That one person who always seems to know everything. Three weeks later, they found it. And they thought: I'd rather just be hungry."

No script needed beyond this — let the room laugh, let it land, then:

> "Every single one of you has been this caveman. I have too. And this talk is about why that keeps happening — and what we can do about it."

**Why this works:**
- Every person in the room (DS and manager) has lived this hunt
- The humour disarms any defensiveness — the caveman is all of us, not a critique
- "I'd rather just be hungry" is a punchline that will travel — people will repeat it later
- Sets up the contrast that runs through the whole talk: hunting vs. a system that just works

**Goal of these slides:** Create shared recognition before any concept is introduced. This is a known pain, not a lecture.

---

## Section 2 — What Changed (1 min)

**Visual concept — two moments:**

**Slide 2A — "How it was" (pre-January 2026)**
Caveman at a laptop, writing on what looks like a cave wall. Speech bubble:
> *"Me writes for me. Me writes for you. Humans together stronger."*

Icons around him: Confluence, Google, Stack Overflow, a colleague. The information ecosystem was entirely human-to-human. Search engines surfaced it. Articles explained it. People shared it. Everything was written by humans, for humans to read.

**The documentation culture that came with it** (spoken, or a brief bullet list on slide):
- Written one-off, in whatever format felt right to the author at the time
- No consistency in structure, naming, depth, or when it was written
- Functioned more as a personal diary than a shared knowledge base — useful if *you* needed to remember something from a year ago, not useful if someone else needed to find it
- At best: written with genuine intention to leave a legacy, but rarely maintained after the project moved on
- At worst: treated as a chore — something to tick off before closing a ticket, not something designed to be read

> "The cave paintings weren't wrong. They captured real things. But they were painted for the painter — not for the next person who might need to find that mammoth."

**Slide 2B — "January 2026"**
A timestamp appears: **January 2026 — Claude Code.**

Brief talking points (spoken, not on slide):
- Claude Code wasn't the first coding assistant, but it showed something new at scale: an agent that *navigates* your repository before it writes a single line
- It reads your `README`, your comments, your folder structure, your conventions — and uses all of it
- Around the same time: Atlassian Rovo started surfacing Confluence knowledge for agents. GitHub Copilot deepened repo context. The pattern was the same everywhere.
- Primary use case was coding — and that's mostly what people noticed. But what actually changed was the **information retrieval layer**.

> "These tools weren't just answering questions. They were reading our institutional context — whether we designed it for them or not."

**The reveal** (the moment the talk pivots):

> "Until January 2026, the only consumers of our documentation were humans. That's no longer true."

The cave wall is the same. The caveman wrote it for other cavemen. But now something else is reading it too — and it doesn't know that the Confluence page hasn't been updated in 18 months.

> "Every repo you work in, every project you run — an agent is either helped or hindered by how you've structured what's in it."

**Goal of these slides:** Shift frame. This isn't AI in the abstract. It's a specific moment that already happened — and it changed who our documentation is written for.

---

## Section 3 — What Is Institutional AI? (1.5 min)

**Talking point:** Give it a name and a simple definition.

> **Institutional AI** is the practice of designing, capturing, and maintaining organisational knowledge so that both humans and AI agents can use it effectively.

It's not about building AI systems. It's about building the *substrate* that makes AI systems useful in our context.

The key mental shift:

| Before | After |
|---|---|
| Documentation (written for humans, read rarely) | Information (structured for both humans and agents, used continuously) |
| Knowledge lives in heads and Confluence | Knowledge lives in structured, navigable, maintained layers |
| 1 person knows a thing | That thing is accessible to everyone — and every agent |

**Goal of this slide:** Land the definition clearly. Not jargon. Something they can repeat.

---

## Section 4 — Examples (2.5 min)

Three short examples. Each one should feel *immediately recognisable*.

### Example A — Onboarding

**Old model:** A new DS joins a project. They spend the first two weeks asking questions, reading outdated docs, reverse-engineering decisions from code comments.

**New model:** The project has a structured context layer — what the project is, why key decisions were made, what the data means, what's known to be broken. A new DS (or an agent assisting them) can get oriented in hours.

*The investment: one structured file, maintained incrementally.*

---

### Example B — Data Knowledge

**Old model:** A DS needs to understand a new dataset before building a model. They ask the one person who knows: about the edge cases, the Pareto rules in the data, the quirks in a certain column, the fact that certain values behave differently in specific conditions. That knowledge lives in one or two people's heads. If they leave or are busy, the DS makes avoidable mistakes.

**New model:** Every project has a structured data context layer — accessible to anyone from day one:
- Links to the ETL code that produces the data
- Performance patterns at a glance: the Pareto rules, the 20% of values that drive 80% of the signal
- Pointers to table catalogues in Unity Catalog, with schema and ownership clearly labelled
- The semantic layer: what the metrics actually mean, how they're defined, what the known discrepancies are
- The quirks: the columns that behave unexpectedly, the edge cases that have burned people before

A new DS (or an agent) can navigate it without burning anyone's time. The knowledge that used to leave with the expert stays in the system.

*The investment: a data card, maintained as the dataset evolves — not a document nobody reads, but the reference layer agents and people reach for first.*

---

### Example C — Modelling Standards and Model Discoverability

**Old model:** How we evaluate models, what metrics matter, how we document experiments — informal and inconsistent. Conventions live in the heads of senior DS or scattered across old notebooks. Models built last year are impossible to reproduce or compare against. A new DS has no way of knowing what exists, let alone how well it performs.

**New model:** Evaluation is repeatable and documented. Models are discoverable — the way HuggingFace works, where every model has a card: what it does, how it was evaluated, what data it used, known limitations. A DS joining a team can see what exists, understand how it performs, and build on it rather than starting from scratch.

*The investment: model cards, evaluation logs, structured experiment tracking. Not bureaucracy — a foundation for trust and reuse.*

> **The leverage mechanism across all three examples:** A **skill** is a packaged, reusable workflow that captures how to do something — evaluating a model, validating a dataset, onboarding onto a new project. One person builds it; everyone (and every agent) benefits.

---

## Section 5 — Skills as Leverage (1 min)

**Talking point:** One of the most powerful tools in this shift is the **skill** — a packaged, reusable, testable workflow.

Think about work that repeats: running a model evaluation, validating a dataset, checking a new project against discipline standards, onboarding onto an unfamiliar data domain. Today, each of these relies on one person knowing how to do it.

A skill packages that knowledge — the steps, the expected inputs, the checks — so that:
- Any DS can run it, not just the person who built it
- An agent can invoke it as part of a larger workflow
- It can be improved centrally and everyone benefits immediately

> "The same week of work that once created tribal knowledge can instead create a skill. The difference: one helps one person once. The other helps everyone, every time."

**Goal of this slide:** Introduce skills as the concrete mechanism for compounding. Not abstract — something we can start building next quarter.

---

## Section 6 — How Agents Navigate: Hierarchy Before Search (1 min)

**Talking point:** A common misconception is that making knowledge "AI-ready" means dumping everything into a search index. It doesn't. The most effective pattern is **hierarchical navigation** — the same way a librarian uses a catalogue before walking to the shelf.

How it works in practice:

1. **Discipline level** — an index that maps the knowledge landscape: what exists, what teams own what, what the shared vocabulary is
2. **Team level** — a context file: what this team builds, how they work, what standards apply
3. **Project level** — a structured README, decision log, data card: what this project is, why key choices were made

An agent (or a new DS) lands at the top, reads the index, navigates to what's relevant, and loads only that. It never needs to read everything at once.

> "Structure isn't documentation overhead. It's navigation infrastructure. The index files and context layers you build today are what allow an agent — or a new DS — to find the right door."

**Goal of this slide:** Explain why *how* information is structured matters as much as its content. This reframes the investment in AGENTS.md files, directory indexes, and metadata: not writing more, but writing in a way that navigates.

---

## Section 7 — Where Are We Now? The Maturity Model (1.5 min)

**Talking point:** It helps to name where most teams currently sit — and to see the path forward as a series of concrete stages, not a cliff.

| Stage | What it looks like | The gap |
|---|---|---|
| **Ad hoc** | Knowledge in heads, Slack archaeology, stale Confluence | Agents and new joiners cannot navigate reliably |
| **Readable** | Repos explain purpose, structure, ownership | Agents can summarise, but still guess what's current |
| **Retrievable** | Knowledge is structured, machine-filterable, navigable | Agents find text — but not always the *right* text |
| **Verifiable** | Key knowledge has freshness checks, contracts, owners | Agents retrieve current, trustworthy information |
| **Agent-operable** | Repeated workflows packaged as skills, outputs auditable | Agents *do things* reliably, not just answer questions |

> "Most of us today are somewhere between Ad hoc and Readable. The goal isn't to jump to Agent-operable in one move. It's to know which stage we're at — and what one step forward looks like."

Every improvement at any stage has value independently of AI. Better structure means faster onboarding. Better metadata means fewer "who owns this?" Slack messages. Verifiable knowledge means less time debugging stale assumptions.

**Goal of this slide:** Make the journey concrete and non-overwhelming. Show that every step forward is valuable — and that work already done counts.

---

## Section 8 — The Compounding Effect (1 min)

**Talking point:** This is the vision argument. Make it feel real.

> "Before: one person does one thing. The value of that work is bounded by how often someone else finds it, understands it, and builds on it. In practice, it rarely compounds."

> "After: one person deposits structured knowledge. Every future person and agent in that context inherits it, builds on it, and extends it. The same hour of work multiplies."

Use a simple visual: a funnel vs. a flywheel.

- **Funnel**: Knowledge created → rarely reused → mostly lost
- **Flywheel**: Knowledge created → structured → surfaced → reused → extended → creates more value

The only thing between the funnel and the flywheel is *how* you capture what you know.

**Goal of this slide:** Make the ROI case. This isn't more work. It's the same work, differently shaped.

---

## Section 9 — Three Levels (1 min)

**Talking point:** Institutional knowledge isn't just one thing. It operates at different scopes.

| Level | What it includes | Who benefits |
|---|---|---|
| **Project** | Context files, decision logs, data contracts, model cards | DS on the project, future DS, agents working on the project |
| **Team** | Conventions, shared practices, team-specific agent instructions | New team members, cross-team collaborators, team-level agents |
| **Discipline** | Shared standards, knowledge base, cross-cutting patterns | Everyone in the discipline, organisation-wide agents |

The vision: we invest at all three levels, and the discipline operates with a shared intelligent context layer beneath it.

**Goal of this slide:** Show scope. This isn't a single project experiment. It's an architecture for the discipline.

---

## Section 10 — The Future Vision (1 min)

**Talking point:** Paint the picture of what we're building toward — grounded, not utopian.

> "Imagine a new data scientist joins the discipline. Within their first week, they can query the discipline's knowledge base, get oriented on how we work, understand the projects relevant to them, and start contributing — without asking anyone to set time aside."

> "Imagine your documentation actually reflects reality. Not because someone had time to update it, but because agents maintain it continuously — flagging when code changes break documented assumptions, updating data cards when schemas drift, keeping the lineage current. Your job shifts from writing documentation to reviewing it, refining it, adding the edge cases and lineage learnings that only you would know."

> "Imagine the question 'how is this model performing?' takes 30 seconds instead of a morning. The weekly performance report someone manually assembles every Friday — gone. Tedious, repetitive monitoring handled. Your time goes to the interpretation, the decisions, the anomalies that actually need a human brain."

> "Imagine two teams never solving the same problem twice. Today, work done in one team rarely travels — it lives in a repo someone else doesn't know exists, or in the head of someone who's moved on. Imagine a DS starting a new modelling problem, searching the discipline's knowledge base, and finding that another team already explored it six months ago — what they tried, what worked, what didn't. They build on it instead of starting from zero. The discipline gets smarter with every project, not just the team that ran it."

These aren't distant possibilities. They're accessible if we change how we think about what we produce.

**Goal of this slide:** Aspiration. Make them want it.

---

## Section 11 — 3 Short-Term Goals (1.5 min)

**Framing (spoken):** These aren't discipline-wide commitments. They're three things a small cross-team group can do in the next six months to learn what works — before we go wider.

---

**Goal 1 — Start at the project level**

Before we build anything at team or discipline level, we need to understand what works. How do agents actually navigate project-level information? What formats hold up? What habits stick? One level at a time, learned properly before scaling.

*Why this first:* We can't jump to team or discipline level without learning what compounds and what doesn't. Long-running projects are the best candidates — the most knowledge to capture, the most to gain.

---

**Goal 2 — Three things in every active project repo**

Concrete and achievable. For each project in the group, add:
- A **data layer reference** — schemas, quirks, Unity Catalog pointers, Pareto patterns
- An **experiment and iteration log** — what we tried, what we learned, what we'd do differently
- At least one **skill** — a reusable, invokable workflow that repeats on the project (evaluation, data validation, anything that runs more than once)

*Why this matters:* This is the deposit. Without it, there's nothing for agents — or future teammates — to navigate.

---

**Goal 3 — Build a weekly freshness agent**

A lightweight agent that runs weekly across the group's projects and checks:
- Data references still point to live tables and schemas
- Model cards exist for every active model and haven't gone stale
- Experiment logs cover recent iterations

The agent flags — it doesn't fix. A weekly digest surfaces what's drifted; a human decides what to do about it. This is the right first posture: build trust in the system before giving it more autonomy.

*Why this matters:* Goal 2 is about depositing knowledge. Goal 3 is about keeping it alive. It's also the first step toward the vision in this talk — documentation that actually reflects reality, not just good intentions.

---

**Call to action**

> *"If this resonates — especially if you're on a long-running project with accumulated knowledge worth capturing — I'd love to hear from you. I want to form a small group from different projects to share learnings together, figure out what works, and build this up before we go wider. Come find me after, or drop me a message."*

---

## Section 12 — Close (30 sec)

**Talking point:** End on the mental model shift, not the to-do list.

> "We've spent years building documentation for humans. We're entering a period where that knowledge also needs to work for agents. The good news is: the same discipline that makes documentation useful for humans — clarity, structure, maintenance — is exactly what makes it useful for agents too."

> "This isn't a transformation programme. It's a mental shift, applied incrementally. And it starts with what we choose to capture next."

---

## Related Artefacts

- **Confluence page (DS People Managers):** [Institutional AI: Building Knowledge That Compounds](https://skyscanner.atlassian.net/wiki/spaces/DSTeam/pages/2592147004/Institutional+AI+Building+Knowledge+That+Compounds) — 5-minute brief for managers covering definition, maturity levels, examples, next phase, and asking for their input on the vision.

---

## Open Questions / Things to Resolve

- [ ] What are the final 3 goals? (options are drafted — needs a decision)
- [ ] Do we want a specific example from our actual work to anchor Examples A/B/C?
- [ ] Is there a concrete number or stat we can use for the compounding argument? (e.g. % of time spent searching for information)
- [ ] Do we show a diagram for the flywheel / three levels?
- [ ] What is the single strongest "before/after" the audience will remember?
- [ ] Do we name the discipline's current pain (Confluence graveyard, knowledge silos)? Or keep it general?

---

## Rejected / Parked Ideas

- Starting with an AI industry overview (too generic, audience doesn't need it)
- Detailed architecture diagram of an agent system (too technical for the tone)
- Case studies from other companies (feels abstract — better to use our own examples)
- Comparing tool options (not the point of this talk)

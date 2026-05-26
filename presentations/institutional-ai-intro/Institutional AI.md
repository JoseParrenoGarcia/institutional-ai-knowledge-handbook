# Institutional knowledge

## Agenda

1. A hunting story
2. What is Institutional Knowledge
3. Institutional knowledge examples
4. Institutional knowledge granularities
5. Maturity levels
6. The future vision
7. 3 short term goals
8. How can you help!

---

## Section 1 — A hunting story

### The old hunt (slides 3–5)

Once upon a time there was a Data Scientist looking for an answer. Questions hanging in the air:

- Has anyone in the discipline already solved something like this?
- Why did we choose to go with survival models?
- What do I need to know about this dataset before I start?

Eventually, after 4 weeks, he found the answer…

> "Bah, I'd rather be hungry than go through this again."

Everyone of you has been this caveman/cavewoman. I have too. This talk is about why that keeps happening and what we can do about it.

### The new hunt (slides 6–8)

**Mid 2025, 17:14, Valencia, Spain — Pre-Claude era**
*Me writes for me. Me writes for you. Humans together stronger.*

Documentation looked like this:
- Written one-off, in whatever format felt right to the author at the time
- No consistency in structure, naming, depth, or when it was written
- Functioned more as a personal diary than a shared knowledge base — useful if you needed to remember something from a year ago, not useful if someone else needed to find it

At best… written with genuine intention to leave a legacy, but rarely maintained after the project moved on. At worst… treated as a chore, something to tick off before closing a ticket, not something designed to be read.

**Mid 2026, 17:14, Valencia, Spain — Post-Claude era**
*Me writes for Agent. Agent helps human. Agents and Humans together stronger.*

Documentation looks like this:
- Claude.md and index.md(s) provide informational hierarchy structures to all repositories
- Agents self-document guided by the user and consistency of information is improved
- Functions as a knowledge base elevating the human and providing other agents quality context for better collaboration

At best… agents are the engine running future information hierarchy, putting the human in the steering wheel. At worst… information is easily retrieved and humans peer-review the informational structure.

---

## Section 2 — What is Institutional Knowledge? (slides 9–12)

The practice of designing, capturing, and maintaining organisational knowledge so that both humans and AI agents can use it effectively.

**The goal: Tribal knowledge.** Only through tribal knowledge can we compound our efforts. AI is an amazing opportunity to rethink how we capture our collective knowledge so that everyone benefits from it.

| | Documentation | Information |
|---|---|---|
| written for | humans, read rarely | structured for both humans & agents, used continuously |
| knowledge lives in | heads, Confluence, and comments in git repos | structured, navigable, maintained layers |
| access | 1 person knows a thing | that thing is accessible to everyone and every agent |

---

## Section 3 — Institutional Knowledge examples (slides 13–15)

**Onboarding** — The project has a structured context layer: what the project is, why key decisions were made, what the data means, what's known to be broken. A new DS and agents can get oriented in hours.

**Data Knowledge** — Every project has a structured data context layer:
- Links to the ETL code that produces the data
- Performance patterns at a glance: the Pareto rules, the 20% of values that drive 80% of the signal
- Pointers to table catalogues in Unity Catalog

**Model Discoverability** — Evaluation is repeatable and documented. Models are discoverable (HuggingFace model card examples). A DS and agents see what exists, has a historical trace, understand how it performs, and build on it rather than starting from scratch.

**Real examples from the discipline:**

- **Alvaro** — 2 different repos, similar analyst skill. Helps answer quick questions that would have taken a few hours to query using SQL and Databricks.
- **James** — Car wiki. A first attempt at capturing both previous ML iterations and future ones in a standard way for agents to learn from the past.
- **Cristobal** — Opex on steroids. Everyone benefits from his agent workflow. A great example of how a discipline can raise the bar across the board.
- And many more: experimentation plugin by Erkam, ads simulator by Ross, Streamlit dashboards for Glazed Donuts.

> The examples exist locally — what we need is to go Tribal.

---

## Section 4 — Granularities (slides 16–17)

Institutional knowledge can be applied at different granularities.

| | project level | team level | discipline level |
|---|---|---|---|
| what | context files, decision logs, data contracts, model cards | conventions, shared practices, indexed project catalog | shared standards, knowledge base, cross-cutting patterns |
| who benefits | DS on the project, future DS, agents working on the project | new team members, cross-team collaborators, team-level agents | everyone in the discipline, organisation-wide agents |

---

## Section 5 — Maturity levels (slides 18–19)

**Where are we now?**

Every improvement at any stage has value independently of AI. We don't need to make the jump to agent-operable in one go.

| stage | what it looks like | the gap |
|---|---|---|
| ad hoc | knowledge in heads, Slack archaeology, stale Confluence | agents and new joiners cannot navigate reliably |
| readable | repos explain purpose, structure, ownership | agents can summarise, but still guess what's current |
| retrievable | knowledge is structured, machine-filterable, navigable | agents find text — but not always the right text |
| verifiable | key knowledge has freshness checks, contracts, owners | agents retrieve current, trustworthy information |
| agent-operable | repeated workflows packaged as skills, outputs auditable | agents do things reliably, not just answer questions |

Most of us are here: some Claude.md files, some skills. But no information hierarchy, no importing our existing knowledge inside repos, no collaboration on improving and evaluating the skills.

---

## Section 6 — The future vision (slides 20–21)

*When every project makes the discipline smarter — that's an idea worth chasing.*

**Imagine a new data scientist joins the discipline.** Within their first week, they can query the discipline's knowledge base, get oriented on how we work, understand the projects relevant to them, and start contributing.

**Imagine your documentation actually reflects reality** because agents maintain it continuously — flagging when code changes break documented assumptions, updating data cards, keeping the lineage current. Your job shifts from writing documentation to reviewing it, refining it, adding the edge cases and lineage learnings that only you would know.

**Imagine the question "how is this model performing?" takes 30 seconds instead of a morning.** The weekly performance report someone manually assembles every Friday, gone. Tedious, repetitive monitoring handled. Your time goes to the interpretation, the decisions, the anomalies that actually need a human brain.

**Imagine a DS starting a new modelling problem**, searching the discipline's knowledge base, and finding that another team already explored it six months ago — what they tried, what worked, what didn't. They build on it instead of starting from zero. The discipline gets smarter with every project, not just the team that ran it.

---

## Section 7 — 3 short-term goals (slides 22–24)

*Explore the foundations — 6 months*

**Goal 1 — Start at the project level.** Before we build anything at team or discipline level, we need to understand what works: how do agents actually navigate project-level information? What formats hold up? What habits stick and which ones don't?

**Goal 2 — 3 things in test project repos:**
1. A data layer reference (schemas, quirks, UC pointers, Pareto patterns)
2. An experiment/iteration log (what we tried, what we learned, what we'd do differently)
3. At least one skill — a reusable workflow others can invoke (evaluation, data validation, anything that repeats)

**Goal 3 — Build a quality & freshness agent.** A lightweight agent that runs weekly across the group's projects and checks: data references still point to live valid tables and schemas; model cards and experiment design docs exist and meet quality standards. The agent flags, it doesn't fix.

**Enthusiasts needed!** I want to form a small group from different projects to share learnings together and figure out what works before we go wider. If this resonates — especially if you're on a long-running project with accumulated knowledge worth capturing — I'd love to hear from you.

---

## Northstar (slide 25)

*Tribal knowledge — Humans and agents together stronger.*

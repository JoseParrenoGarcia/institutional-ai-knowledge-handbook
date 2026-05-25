# Brainstorm — Institutional AI: The Discipline Presentation

> **Stage:** Initial brainstorm — flow and talking points, not final copy
> **Constraint:** ~10 minutes. Target 8–10 slides. No fluff.

---

## Narrative Arc

The talk needs a single emotional thread: *"Our work is about to compound in ways it never could before — but only if we change something small about how we think about knowledge."*

Open with a recognition moment (something they've all experienced). Build to a vision. Land on three things they can do next week.

---

## Section 1 — The Hook (1 min)

**Talking point:** Start with a moment everyone has lived.

> "When was the last time you spent 30 minutes hunting for something you knew existed — a decision someone made on a project, how we approached a certain problem, why a model was built a certain way — and either never found it or found it buried in a Confluence page nobody had touched in 18 months?"

The problem isn't that we don't write things down. The problem is we write them *for ourselves*, in the moment, in formats that don't survive handover.

**Goal of this slide:** Create shared recognition. This is a known pain, not a lecture.

---

## Section 2 — What Changed (1 min)

**Talking point:** The tools we now use are reading our institutional context whether we design it or not.

- GitHub Copilot is reading our repo structure, our READMEs, our comments
- AI assistants are searching our docs, our Slack, our Confluence
- Agents being built today will be orchestrated across our data platform

The difference: until now, **only humans** were the consumers of our documentation. That's no longer true.

> "Every repo you work in, every project you run — an agent is either helped or hindered by how you've structured what's in it."

**Goal of this slide:** Shift frame. This isn't about AI in the abstract. It's about what's already happening.

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

## Section 4 — Examples (2 min)

Three short examples. Each one should feel *immediately recognisable*.

### Example A — Onboarding

**Old model:** A new DS joins a project. They spend the first two weeks asking questions, reading outdated docs, reverse-engineering decisions from code comments.

**New model:** The project has a structured context layer — what the project is, why key decisions were made, what the data means, what's known to be broken. A new DS (or an agent assisting them) can get oriented in hours.

*The investment: one structured file, maintained incrementally.*

---

### Example B — Project Handover

**Old model:** Person leaves or rotates off. There's a handover doc. It's out of date by the time it's written. The knowledge leaves with the person.

**New model:** Knowledge is captured continuously at the point of work — decision logs, model cards, context files. The "handover" is just pointing at what already exists.

*The investment: the habit of depositing, not just producing.*

---

### Example C — Discipline Standards

**Old model:** Code review guidelines, modelling conventions, data quality standards — all in Confluence. Known by the people who wrote them. Rediscovered or ignored by everyone else.

**New model:** Standards are machine-readable. An agent can check a new project against them. A DS can query them. New joiners find them without asking.

*The investment: structured, not buried.*

---

## Section 5 — The Compounding Effect (1 min)

**Talking point:** This is the vision argument. Make it feel real.

> "Before: one person does one thing. The value of that work is bounded by how often someone else finds it, understands it, and builds on it. In practice, it rarely compounds."

> "After: one person deposits structured knowledge. Every future person and agent in that context inherits it, builds on it, and extends it. The same hour of work multiplies."

Use a simple visual: a funnel vs. a flywheel.

- **Funnel**: Knowledge created → rarely reused → mostly lost
- **Flywheel**: Knowledge created → structured → surfaced → reused → extended → creates more value

The only thing between the funnel and the flywheel is *how* you capture what you know.

**Goal of this slide:** Make the ROI case. This isn't more work. It's the same work, differently shaped.

---

## Section 6 — Three Levels (1 min)

**Talking point:** Institutional knowledge isn't just one thing. It operates at different scopes.

| Level | What it includes | Who benefits |
|---|---|---|
| **Project** | Context files, decision logs, data contracts, model cards | DS on the project, future DS, agents working on the project |
| **Team** | Conventions, shared practices, team-specific agent instructions | New team members, cross-team collaborators, team-level agents |
| **Discipline** | Shared standards, knowledge base, cross-cutting patterns | Everyone in the discipline, organisation-wide agents |

The vision: we invest at all three levels, and the discipline operates with a shared intelligent context layer beneath it.

**Goal of this slide:** Show scope. This isn't a single project experiment. It's an architecture for the discipline.

---

## Section 7 — The Future Vision (1 min)

**Talking point:** Paint the picture of what we're building toward — grounded, not utopian.

> "Imagine a new data scientist joins the discipline. Within their first day, they can query the discipline's knowledge base, get oriented on how we work, understand the projects relevant to them, and start contributing — without asking anyone to set time aside."

> "Imagine a project that's been running for three years. A team member leaves. The work continues without a knowledge gap, because the knowledge was never just in that person's head."

> "Imagine our standards not being something you have to remember or look up — they're embedded in the tools and agents that help us work."

These aren't distant possibilities. They're accessible if we change how we think about what we produce.

**Goal of this slide:** Aspiration. Make them want it.

---

## Section 8 — 3 Short-Term Goals (1.5 min)

> **[DRAFT — options to discuss and refine]**

The following are candidate goals. Select or refine three that feel right given what's achievable in the next quarter.

**Option A — Audit what we have**
> Map our current documentation across Confluence, repos, and shared drives. Identify what's structured vs. buried. Establish a baseline before we improve anything.

**Option B — Pilot project-level context files**
> One team picks 2–3 active projects and adds a structured context layer (a `README` with a defined schema, a decision log, a data contract). Run it for 6 weeks and report back.

**Option C — Define the knowledge architecture**
> Run a working session to agree what institutional knowledge means for our discipline — what levels we operate at, what format we use, who maintains what.

**Option D — One knowledge experiment**
> Identify one high-pain knowledge problem (onboarding, standards access, project handover) and solve it with structured information. Measure the before/after.

**Option E — Agents.md for every active project**
> Every active project gets a machine-readable context file by end of quarter. Establish what goes in it, and make it part of the project start checklist.

*Recommendation: pick goals that span exploration (understanding what we have), definition (agreeing what we want), and action (one concrete pilot).*

---

## Section 9 — Close (30 sec)

**Talking point:** End on the mental model shift, not the to-do list.

> "We've spent years building documentation for humans. We're entering a period where that knowledge also needs to work for agents. The good news is: the same discipline that makes documentation useful for humans — clarity, structure, maintenance — is exactly what makes it useful for agents too."

> "This isn't a transformation programme. It's a mental shift, applied incrementally. And it starts with what we choose to capture next."

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

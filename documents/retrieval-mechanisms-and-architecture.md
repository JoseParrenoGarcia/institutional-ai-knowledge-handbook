---
theme: retrieval-mechanisms-and-architecture
document_type: institutional_ai_research_report
generated_date: 2026-05-25
canonical_format: markdown
---

# Retrieval Mechanisms and Architecture

This report examines the rapidly evolving landscape of retrieval architectures for AI agents, focusing on repository-aware retrieval, agentic RAG systems, semantic indexing, graph-based context selection, hierarchical repository decomposition, and operational retrieval infrastructure. The research synthesises emerging production patterns across engineering systems, open-source frameworks, coding agents, and retrieval-focused AI architectures relevant to DS/ML organisations, platform teams, and institutional AI infrastructure.

---

# Executive Summary

Retrieval has quietly become one of the defining infrastructure problems of institutional AI systems.

The industry discussion often frames retrieval as a subcomponent of RAG pipelines:
- embeddings,
- vector databases,
- chunking,
- reranking,
- and semantic search.

The reviewed sources suggest something much broader.

Modern retrieval systems are increasingly evolving into:
- orchestration architectures,
- repository navigation systems,
- operational context engines,
- and dynamic reasoning substrates for agents.

The strongest pattern across the ecosystem is that retrieval is shifting from:
“fetching documents”
towards:
“constructing executable operational context”.

This distinction matters profoundly.

Traditional RAG systems treated retrieval as:
- a one-shot query operation,
- typically embedding-based,
- with relatively static chunk retrieval.

The newer generation of systems increasingly treats retrieval as:
- iterative,
- stateful,
- graph-aware,
- hierarchical,
- tool-augmented,
- and dynamically self-correcting.

The shift towards “agentic retrieval” is therefore not merely about better search.

It is about turning retrieval into an active reasoning process.

Several strong patterns recur across the reviewed sources.

## 1. Retrieval Is Becoming Graph-Oriented Rather Than Chunk-Oriented

One of the clearest trends is the move away from naïve chunk retrieval towards structural repository understanding.

Several sources independently converge on graph-based retrieval architectures:
- symbol graphs,
- dependency graphs,
- repository maps,
- hierarchical decomposition,
- call graphs,
- and semantic linkage systems.

This is particularly visible in:
- Aider RepoMap,
- Hermes PageRank proposals,
- and CodeWiki-style decomposition systems.

The key operational insight is that:
repositories are not flat text corpora.

They are structured dependency systems.

Embedding-based chunk retrieval alone performs poorly when:
- architectural understanding,
- cross-file relationships,
- dependency tracing,
- or operational workflows
matter.

Graph-aware retrieval architectures attempt to preserve:
- structural coherence,
- contextual locality,
- semantic linkage,
- and operational dependencies.

This appears increasingly necessary for:
- code agents,
- platform agents,
- experiment reproduction systems,
- and institutional workflow automation.

## 2. Hierarchical Decomposition Is Emerging as a Core Pattern

Another strong recurring idea is hierarchical retrieval decomposition.

Several sources independently advocate:
- repository partitioning,
- multi-level summarisation,
- module-level abstraction,
- recursive retrieval,
- and layered context expansion.

The motivation is both practical and architectural.

Large repositories exceed:
- token budgets,
- reasoning stability,
- and retrieval precision limits.

Hierarchical decomposition therefore acts as:
- a compression strategy,
- a retrieval control mechanism,
- and an operational abstraction layer.

The strongest systems progressively expand context:
1. high-level architecture,
2. subsystem summaries,
3. targeted modules,
4. implementation detail.

This resembles classic systems engineering approaches more than traditional document retrieval.

One begins to suspect that computer science keeps rediscovering hierarchy because hierarchy remains stubbornly useful.

## 3. Agentic Retrieval Is Replacing Static Retrieval

The Hex “Agentic RAG” article is important because it captures a broader architectural transition:
retrieval is increasingly being integrated into agent orchestration loops.

The defining characteristics include:
- iterative retrieval,
- self-correction,
- tool orchestration,
- retrieval planning,
- dynamic query refinement,
- and multi-step reasoning.

The important operational distinction is:
the agent decides what additional context it requires during execution.

This is qualitatively different from classic:
“retrieve top-k chunks and hope for the best”.

The architectural implications are substantial:
retrieval becomes:
- adaptive,
- stateful,
- and execution-aware.

However, this also introduces:
- observability challenges,
- governance complexity,
- cost unpredictability,
- and new failure modes.

## 4. Retrieval Quality Increasingly Depends on Structural Metadata

A recurring lesson across all sources is that:
retrieval quality depends heavily on structural information rather than embeddings alone.

Effective systems increasingly combine:
- semantic retrieval,
- exact search,
- symbol indexing,
- dependency analysis,
- repository graphs,
- metadata filters,
- and architectural hierarchy.

This aligns with broader production observations:
vector similarity alone is often insufficient for operational correctness.

The strongest systems therefore implement:
hybrid retrieval architectures.

## 5. Token Budgets Are Becoming Architectural Constraints

Several sources explicitly frame token budgets as infrastructure constraints rather than model limitations.

This is operationally important.

The practical retrieval challenge is increasingly:
“How do we expose the smallest possible high-quality context?”

The PageRank RepoMap proposal is particularly notable here.

It attempts to:
- prioritise structurally relevant files,
- compress repository representations,
- and dynamically allocate context budgets.

This resembles:
- search engine ranking,
- graph centrality algorithms,
- and compiler dependency analysis
far more than classical document retrieval.

The retrieval layer is quietly becoming an operating system for context management.

## 6. Semantic Indexing Is Becoming Team Infrastructure

The Cursor secure indexing article highlights another emerging trend:
semantic repository indexing is becoming shared organisational infrastructure.

The important operational shift is that:
repository indexing is no longer viewed as a local optimisation.

It is increasingly treated as:
- persistent team infrastructure,
- shared context acceleration,
- and onboarding optimisation.

This introduces important concerns around:
- cache invalidation,
- freshness,
- index consistency,
- security,
- and access control.

The use of Merkle trees for repository change detection is particularly notable because it imports distributed systems ideas directly into retrieval infrastructure.

This is probably a sensible sign.

## 7. Retrieval Systems Are Becoming Governance Systems

An important but less explicit pattern is that retrieval architectures increasingly define:
- operational visibility,
- context boundaries,
- access constraints,
- and knowledge exposure.

Retrieval is therefore becoming a governance layer.

This matters enormously for institutional AI because:
- retrieval scope determines agent capability,
- context exposure determines operational risk,
- and indexing quality determines organisational trust.

The retrieval layer is not merely a performance optimisation.

It is increasingly a control surface.

## Production Readiness Assessment

The strongest production-ready patterns appear to be:
- hybrid retrieval,
- repository maps,
- semantic indexing,
- graph-assisted retrieval,
- dependency-aware ranking,
- and hierarchical decomposition.

Moderately mature but evolving:
- agentic retrieval orchestration,
- dynamic retrieval planning,
- recursive retrieval expansion,
- repository summarisation agents.

Still speculative or operationally immature:
- fully autonomous retrieval planning,
- large-scale graph-native reasoning systems,
- persistent self-maintaining retrieval ecosystems,
- universal repository understanding layers.

The overall direction is increasingly clear:

Retrieval systems are evolving from:
“vector databases with prompts”
towards:
“dynamic operational context infrastructure for agents”.

That is a much more ambitious engineering problem.

And rather less glamorous than many marketing diagrams suggest.

---

# Theme Overview Table

| Title | Link | Type | Signal Strength | Description |
|---|---|---|---|---|
| Agentic RAG Explained: The Next Evolution of Agentic AI | https://hex.tech/blog/agentic-rag-explained/ | Engineering article | High | Explains the transition from static RAG pipelines towards iterative, tool-aware, self-correcting retrieval orchestration systems. |
| CodeWiki: Automated Repository-Level Documentation at Scale | https://arxiv.org/html/2510.24428v1 | Research paper | High | Proposes hierarchical repository decomposition and specialised agent orchestration for large-scale repository understanding and documentation generation. |
| Feature: Code Wiki Skill (GitHub Issue #486) | https://github.com/NousResearch/hermes-agent/issues/486 | GitHub issue / architecture discussion | Medium | Discusses repository walkthrough generation, documentation synthesis, and skill-oriented repository explanation systems for Hermes Agent. |
| Feature: PageRank Repo Map (GitHub Issue #535) | https://github.com/NousResearch/hermes-agent/issues/535 | GitHub issue / architecture proposal | High | Proposes graph-based repository context ranking using Personalized PageRank and directed symbol graphs to optimise token-efficient retrieval. |
| Repository map - Aider | https://aider.chat/docs/repomap.html | Engineering documentation | High | Describes Aider’s repository mapping system for compressed repository understanding using dependency-aware graph ranking. |
| Securely indexing large codebases - Cursor | https://cursor.com/blog/secure-codebase-indexing | Engineering article | High | Details semantic repository indexing infrastructure using Merkle trees, shared indexes, and secure incremental indexing strategies. |
| llm-wiki-compiler | https://github.com/atomicstrata/llm-wiki-compiler | GitHub repository | High | Implements knowledge compilation as a complement to agentic RAG: a two-phase concept extraction and page generation pipeline producing graph-linked wiki artifacts with token-budgeted context packs. |

---

# Source Breakdowns

## Source 4 — Agentic RAG Explained: The Next Evolution of Agentic AI

### Metadata

- Source type: Engineering article
- Signal strength: High
- Primary relevance: Agentic retrieval orchestration
- URL: https://hex.tech/blog/agentic-rag-explained/

### Core argument

The article argues that retrieval systems are evolving from static one-shot retrieval pipelines into dynamic agent-driven retrieval orchestration systems.

The core thesis is that:
effective retrieval increasingly requires:
- iterative reasoning,
- retrieval planning,
- dynamic query refinement,
- and tool-assisted context expansion.

### Key ideas and highlights

Key operational patterns include:
- multi-step retrieval loops,
- self-correcting retrieval,
- retrieval-aware planning,
- dynamic context expansion,
- and adaptive query decomposition.

The article strongly distinguishes:
classic RAG:
- retrieve once,
- answer once

from:
agentic retrieval:
- retrieve,
- reason,
- identify gaps,
- retrieve again,
- validate,
- continue execution.

This introduces retrieval as an active reasoning substrate rather than passive context injection.

The architecture also includes:
- orchestration layers,
- retrieval memory,
- tool coordination,
- and iterative grounding mechanisms.

### Why this matters for institutional AI

Institutional workflows often involve:
- fragmented knowledge,
- multi-step dependencies,
- operational ambiguity,
- and evolving state.

Static retrieval frequently fails in such environments because:
the required context is not known upfront.

Agentic retrieval architectures improve:
- operational adaptability,
- context precision,
- and complex workflow execution.

### Practical implications for DS/ML teams

Practical implications include:
- designing retrieval as a workflow,
- implementing retrieval observability,
- introducing retrieval planning layers,
- and separating retrieval orchestration from reasoning logic.

DS/ML teams should increasingly treat:
retrieval pipelines as operational infrastructure rather than prompt accessories.

### Limitations and caveats

The article is conceptually strong but operationally optimistic.

Key unresolved concerns include:
- retrieval cost explosion,
- orchestration complexity,
- observability challenges,
- debugging difficulty,
- and retrieval instability.

Production governance patterns remain underdeveloped.

---

## Source 7 — CodeWiki: Automated Repository-Level Documentation at Scale

### Metadata

- Source type: Research paper
- Signal strength: High
- Primary relevance: Hierarchical repository decomposition
- URL: https://arxiv.org/html/2510.24428v1

### Core argument

The paper proposes a framework for generating repository-level understanding through hierarchical decomposition and specialised documentation agents.

The central thesis is that:
large repositories require structured decomposition rather than flat summarisation.

### Key ideas and highlights

Key architectural ideas include:
- hierarchical repository partitioning,
- leaf-module analysis,
- architecture synthesis,
- dependency extraction,
- data-flow reconstruction,
- and recursive summarisation.

The framework employs specialised agents responsible for:
- local module understanding,
- relationship extraction,
- and higher-level synthesis.

Important implementation patterns include:
- bottom-up summarisation,
- layered abstraction,
- recursive context aggregation,
- and repository graph analysis.

The system attempts to preserve:
- architectural coherence,
- dependency understanding,
- and subsystem boundaries.

### Why this matters for institutional AI

Large institutional repositories often exceed:
- token limits,
- comprehension limits,
- and retrieval stability.

Hierarchical decomposition offers:
- scalable repository understanding,
- improved retrieval locality,
- and architecture-aware summarisation.

This is particularly important for:
- onboarding,
- architectural analysis,
- dependency tracing,
- and repository governance.

### Practical implications for DS/ML teams

DS/ML teams may benefit from:
- repository partitioning,
- hierarchical retrieval layers,
- architecture-aware indexing,
- and recursive documentation systems.

The approach also supports:
- operational knowledge synthesis,
- dependency-aware retrieval,
- and cross-team onboarding.

### Limitations and caveats

The paper remains relatively experimental.

Operational scalability in:
- very large monorepos,
- rapidly changing repositories,
- and heterogeneous ecosystems
remains uncertain.

Evaluation benchmarks are also somewhat limited compared to mature retrieval systems research.

---

## Source 10 — Feature: Code Wiki Skill (GitHub Issue #486)

### Metadata

- Source type: GitHub architecture discussion
- Signal strength: Medium
- Primary relevance: Repository walkthrough generation
- URL: https://github.com/NousResearch/hermes-agent/issues/486

### Core argument

The issue proposes a “Code Wiki Skill” for Hermes Agent capable of generating:
- walkthroughs,
- sequence diagrams,
- architecture summaries,
- and repository explanations.

The proposal treats repository understanding as a reusable agent skill.

### Key ideas and highlights

Key operational ideas include:
- repository summarisation,
- workflow explanation,
- architecture extraction,
- dependency walkthroughs,
- and diagram generation.

The discussion also references:
- DeepWiki-Open,
- GitDiagram,
- and related repository analysis systems.

A notable pattern is the packaging of repository analysis itself as:
- a reusable operational capability.

This reflects broader ecosystem movement towards:
capability modularisation.

### Why this matters for institutional AI

Institutional repositories increasingly require:
- explainability,
- onboarding acceleration,
- architectural transparency,
- and operational discoverability.

Repository explanation skills can reduce:
- onboarding friction,
- architecture ambiguity,
- and operational dependency blindness.

### Practical implications for DS/ML teams

Potential applications include:
- automated onboarding assistants,
- architecture explainers,
- dependency tracing agents,
- and operational repository walkthrough systems.

The approach also supports:
- institutional knowledge preservation,
- and architectural observability.

### Limitations and caveats

The proposal is conceptual rather than production-validated.

Operational concerns include:
- documentation staleness,
- summarisation hallucination,
- architecture oversimplification,
- and maintenance overhead.

No formal evaluation methodology is yet established.

---

## Source 11 — Feature: PageRank Repo Map (GitHub Issue #535)

### Metadata

- Source type: GitHub architecture proposal
- Signal strength: High
- Primary relevance: Graph-ranked repository retrieval
- URL: https://github.com/NousResearch/hermes-agent/issues/535

### Core argument

The proposal introduces a repository retrieval system based on:
- directed symbol graphs,
- dependency analysis,
- and Personalized PageRank ranking.

The goal is to optimise:
- repository context selection,
- retrieval precision,
- and token efficiency.

### Key ideas and highlights

Important implementation patterns include:
- directed symbol graphs,
- PageRank-style relevance propagation,
- scope-aware retrieval,
- graph-based prioritisation,
- and elided context generation.

The proposal treats repository retrieval similarly to:
- web search ranking,
- dependency analysis,
- and graph centrality modelling.

This is one of the strongest operational retrieval architectures among the reviewed sources.

The approach explicitly recognises:
token budgets as architectural constraints.

### Why this matters for institutional AI

Institutional repositories contain:
- dense dependencies,
- semantic linkage,
- and operational structure
that flat chunk retrieval cannot capture effectively.

Graph-aware ranking improves:
- architectural retrieval,
- dependency-aware reasoning,
- and token allocation efficiency.

### Practical implications for DS/ML teams

Practical applications include:
- repository-aware retrieval layers,
- graph-assisted context ranking,
- architecture-sensitive retrieval pipelines,
- and dependency-aware onboarding systems.

This approach appears highly relevant for:
- large ML platforms,
- feature stores,
- experimentation systems,
- and shared infrastructure repositories.

### Limitations and caveats

The proposal remains early-stage.

Operational complexity may become significant for:
- massive monorepos,
- rapidly evolving repositories,
- or polyglot codebases.

Graph maintenance and freshness also introduce non-trivial infrastructure overhead.

---

## Source 21 — Repository map - Aider

### Metadata

- Source type: Engineering documentation
- Signal strength: High
- Primary relevance: Repository-aware context compression
- URL: https://aider.chat/docs/repomap.html

### Core argument

Aider proposes “RepoMap” as a compressed repository representation enabling agents to understand repository structure without loading entire codebases.

The core thesis is:
agents require structural awareness rather than raw repository ingestion.

### Key ideas and highlights

Key implementation mechanisms include:
- dependency-aware ranking,
- graph-based file prioritisation,
- concise repository mapping,
- and symbol-level retrieval.

The system attempts to expose:
- call signatures,
- dependencies,
- interfaces,
- and repository topology
within constrained token budgets.

Importantly, RepoMap is designed to remain:
- lightweight,
- dynamically generated,
- and operationally useful.

### Why this matters for institutional AI

Institutional repositories frequently exceed:
- context windows,
- stable retrieval limits,
- and operational reasoning capacity.

Compressed repository maps improve:
- onboarding,
- architectural navigation,
- dependency tracing,
- and operational reasoning.

### Practical implications for DS/ML teams

DS/ML teams should consider:
- repository abstraction layers,
- compressed architecture maps,
- graph-aware retrieval,
- and dependency-sensitive indexing.

RepoMap-style systems appear particularly valuable for:
- large ML platforms,
- experimentation systems,
- and operational infrastructure repositories.

### Limitations and caveats

Compressed repository representations may:
- omit subtle implementation detail,
- hide operational edge cases,
- or oversimplify dependency complexity.

The approach also depends heavily on:
- accurate graph extraction,
- repository structure quality,
- and stable indexing infrastructure.

---

## Source 24 — Securely indexing large codebases - Cursor

### Metadata

- Source type: Engineering article
- Signal strength: High
- Primary relevance: Semantic repository indexing infrastructure
- URL: https://cursor.com/blog/secure-codebase-indexing

### Core argument

The article explains how Cursor indexes large repositories using:
- semantic search,
- Merkle trees,
- incremental indexing,
- and secure shared index reuse.

The central thesis is that:
repository indexing should behave like scalable infrastructure rather than ephemeral local tooling.

### Key ideas and highlights

Important implementation patterns include:
- incremental indexing,
- semantic repository search,
- Merkle-tree change detection,
- index sharing,
- cache reuse,
- and secure retrieval acceleration.

The use of Merkle trees is particularly notable because it:
- minimises redundant indexing,
- enables deterministic change tracking,
- and improves scalability.

The architecture strongly emphasises:
- onboarding speed,
- retrieval freshness,
- and operational efficiency.

### Why this matters for institutional AI

Institutional AI systems increasingly depend on:
- persistent semantic indexes,
- repository understanding,
- and retrieval infrastructure.

Index freshness and consistency become operationally critical once:
- agents rely on repository context for execution.

### Practical implications for DS/ML teams

Practical lessons include:
- treating indexing as platform infrastructure,
- implementing incremental indexing,
- separating indexing from execution,
- and introducing secure shared retrieval layers.

This is highly relevant for:
- large engineering organisations,
- multi-repository ML platforms,
- and internal AI assistants.

### Limitations and caveats

The article is engineering-focused rather than academically validated.

Operational trade-offs around:
- index invalidation,
- distributed consistency,
- access governance,
- and retrieval observability
remain partially unresolved.

Still, the infrastructure maturity appears credible.

---

## Source — llm-wiki-compiler (llmwiki)

### Metadata

- Source type: GitHub repository
- Signal strength: High
- Primary relevance: Knowledge compilation as a complementary retrieval philosophy to RAG
- URL: https://github.com/atomicstrata/llm-wiki-compiler

### Core argument

llmwiki implements the knowledge compilation pattern: raw sources are compiled once into a persistent, interlinked markdown wiki. The core retrieval distinction is:

```
RAG:     query → search chunks → answer → forget
llmwiki: sources → compile → wiki → query → save → richer wiki → better answers
```

Rather than re-discovering relationships at query time, the system pre-computes them into a structured artifact. Future queries retrieve from the compiled wiki rather than raw source chunks.

### Key ideas and highlights

Architecturally notable features:

- two-phase pipeline eliminating order-dependence: Phase 1 extracts all concepts from all sources; Phase 2 generates interlinked pages with `[[wikilink]]` resolution;
- context graph packs (v0.8.0): `llmwiki context` and MCP `get_context_pack` produce token-budgeted evidence packs containing primary pages, graph neighbours, citations, optional source windows, warnings, and suggested actions;
- typed page schema: `concept`, `entity`, `comparison`, `overview` — structured retrieval artifacts rather than flat chunks;
- incremental indexing via SHA-256 hash change detection — only changed sources go through the LLM;
- compounding queries: saved query answers become new wiki pages, improving future retrieval context;
- MCP server integration (`llmwiki serve`) makes the compiled wiki directly queryable by agents.

### Why this matters for institutional AI

Knowledge compilation represents a distinct retrieval architecture from agentic RAG:

- RAG is dynamic, stateless, and re-discovers relationships per query;
- compiled wikis are persistent artifacts with explicit graph structure, source attribution, and typed page kinds.

The context graph packs feature is particularly relevant as a retrieval architecture: it provides structured, graph-aware, token-budgeted context delivery — aligned with the broader trend towards retrieval as operational context infrastructure rather than chunk retrieval.

The two are complementary rather than competing. RAG excels at ad-hoc retrieval over large, frequently-updated corpora. Knowledge compilation excels at extracting relational depth from stable, high-signal corpora and accumulating understanding over time.

### Practical implications for DS/ML teams

Operational patterns worth considering:

- compiled wikis as a retrieval substrate for stable, high-signal corpora (papers, design docs, decision records);
- context graph packs as a token-efficient graph-aware context delivery mechanism;
- hash-based incremental indexing as a lightweight alternative to full re-embedding on source changes;
- MCP server integration for agent-queryable institutional wikis.

### Limitations and caveats

Best suited for small, high-signal corpora. Query routing is index-based rather than full graph traversal, limiting recall for loosely-structured corpora. An evaluation harness benchmarking against retrieval baselines is on the roadmap rather than implemented. Production-scale adoption evidence remains limited.

---

# Appendix — Discarded or Supporting Sources

No sources were fully discarded for this theme. However, several overlap patterns were identified.

| Title | Link | Reason for partial deprioritisation |
|---|---|---|
| Feature: Code Wiki Skill (GitHub Issue #486) | https://github.com/NousResearch/hermes-agent/issues/486 | Conceptually overlaps with the more architecturally developed hierarchical decomposition ideas in CodeWiki. |
| Repository map - Aider | https://aider.chat/docs/repomap.html | Operationally overlaps with the more graph-centric PageRank RepoMap proposal, though still retained for production maturity insights. |

---

# Final Theme Synthesis

## Strongest recurring patterns

The strongest recurring themes are:
- graph-aware retrieval,
- hierarchical decomposition,
- repository-aware indexing,
- dynamic retrieval orchestration,
- and token-efficient context compression.

The ecosystem is converging on:
“retrieval as operational context infrastructure”.

## Most actionable implementation ideas

Highest-value practical ideas include:
- hybrid retrieval architectures,
- repository graph extraction,
- hierarchical indexing,
- dependency-aware ranking,
- semantic repository maps,
- and incremental indexing systems.

These appear deployable today within mature engineering organisations.

## Most speculative or immature ideas

Less mature concepts include:
- fully autonomous retrieval planning,
- universal repository reasoning layers,
- large-scale graph-native retrieval ecosystems,
- and persistent self-maintaining retrieval architectures.

The conceptual direction is promising, but operational governance remains immature.

## Gaps in evidence

Important evidence gaps include:
- large-scale benchmarking,
- retrieval governance studies,
- operational observability standards,
- cost-performance trade-off evaluation,
- and longitudinal retrieval reliability analysis.

Most evidence remains:
- engineering-oriented,
- operationally anecdotal,
- or early-stage architectural research.

## Recommendations for DS/ML organisations

Recommended operational sequence:
1. Introduce semantic indexing infrastructure.
2. Add hybrid retrieval.
3. Implement repository-aware graph extraction.
4. Add hierarchical decomposition.
5. Introduce retrieval observability.
6. Experiment cautiously with agentic retrieval orchestration.

Avoid:
- pure embedding-only retrieval,
- premature GraphRAG complexity,
- and uncontrolled retrieval autonomy.

## What appears production-ready versus experimental

### Production-ready
- Semantic repository indexing
- Hybrid retrieval
- Dependency-aware repository maps
- Incremental indexing
- Graph-assisted ranking
- Hierarchical retrieval

### Emerging but credible
- Agentic retrieval orchestration
- Repository decomposition agents
- Recursive retrieval expansion
- Graph-native context ranking

### Experimental or speculative
- Autonomous retrieval planning
- Persistent self-maintaining retrieval systems
- Fully graph-native reasoning architectures
- Universal repository cognition systems

The strongest operational conclusion is that:
retrieval systems are no longer simply search systems.

They are rapidly becoming:
- reasoning infrastructure,
- governance infrastructure,
- and operational context infrastructure for agents.

That is a much larger systems-engineering challenge than “adding RAG”.

And probably deserves rather more architectural seriousness than it currently receives.
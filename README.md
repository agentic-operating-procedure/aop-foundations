# AOP Foundations

`aop-foundations` is the single authority for what an Agentic Operating Procedure is, what it is not, and the vocabulary used to say so precisely.

| Field | Value |
|---|---|
| Authority | The concept: definition, hierarchy, vocabulary, boundaries |
| Tier | Concept |
| Landing wave | 1 |
| Version | 0.1.1 |
| Status | Stable |
| Licence | MIT |

## What this repository owns

- The founding paper: what an AOP is, how it differs from a Standard Operating Procedure, and why that difference is structural rather than a matter of emphasis.
- The six-level conceptual hierarchy, and the governing principle that the procedure governs the agent.
- The glossary: a stable identifier for every defined term.
- The non-goals and the misconception ladder: the boundaries that keep the concept from collapsing into a neighbouring label.

## What this repository does not own

- The machine-readable model, the identifier scheme, or the conformance clauses. That is `aop-spec`.
- The change process for the estate, or the decision records. That is `aop-governance`.
- The comparison against adjacent disciplines. That is `aop-landscape`.

The distinction matters because a concept that is also a model, a process, and a comparison cannot be maintained. Each of those has its own rate of change and its own authority, so each has its own repository.

## The concept in one page

An Agentic Operating Procedure is a structured operational specification that defines how agents may interpret intent, make decisions, coordinate capabilities and execute actions within explicitly governed operational boundaries, to achieve verifiable outcomes.

A Standard Operating Procedure prescribes a sequence of activities for a human to follow. An AOP establishes the conditions under which an agentic system determines and adapts its own execution path, within an authority boundary that is written down in advance.

The difference shows up in four places.

| | SOP | AOP |
|---|---|---|
| Source | Authored from intent | Compiled from observation |
| Structure | Linear prose describing a corridor | A network of variants, decision points and exception edges |
| Semantics | What should happen | What happens, what the agent may decide about it, and what evidence shows it did |
| Control | Read by a person who may notice something the document missed | Executed by an agent that cannot notice, so the escalation boundary must be written down first |

An SOP is a hypothesis about the work. An AOP is a measurement of it, with provenance.

## The six-level hierarchy

| # | Concept | Architectural responsibility |
|---|---|---|
| 1 | Agentic Operating Engineering | The discipline |
| 2 | Agentic Operating Procedure | The operational specification |
| 3 | Agent Skill | The reusable capability |
| 4 | Domain Agent Harness | The controlled execution environment |
| 5 | Agent | The execution actor |
| 6 | Agentic Operations | The broader operating mode |

Read downwards, the ladder is a discipline: the concept governs how the discipline is practised, the procedure specifies operating intent, the skill packages reusable capability, the harness controls the execution environment, the agent acts, and the operating mode is the regime those actions produce.

Read upwards, it is a containment: the operating mode contains agents, agents run inside a harness, a harness is governed by an AOP, an AOP invokes skills, and the whole apparatus expresses the discipline.

**The procedure governs the agent, not the other way around.** The agent operates within the authority, constraints and assurance requirements the AOP establishes. It cannot self-authorise. The authority check runs in a component outside the model context, so the agent cannot influence the outcome of the check that governs it. Every other design decision in the programme is downstream of this one.

## Documents

| Document | What it settles |
|---|---|
| [`docs/aop-founding-paper-concept-scope.md`](docs/aop-founding-paper-concept-scope.md) | The concept, its origin in procedural engineering, and its relation to SOPs, skills and harnesses |
| [`docs/aop-conceptual-hierarchy-concept-scope.md`](docs/aop-conceptual-hierarchy-concept-scope.md) | The six levels, their architectural responsibilities, and the governing principle |
| [`docs/aop-glossary-concept-scope.md`](docs/aop-glossary-concept-scope.md) | Every defined term, with a stable identifier |
| [`docs/aop-non-goals-concept-scope.md`](docs/aop-non-goals-concept-scope.md) | What the concept is not, and the common misreadings it invites |

## Repository layout

```
aop-foundations/
  README.md            # this file
  CHANGELOG.md         # release notes
  CODEOWNERS           # ownership
  LICENSE              # MIT
  docs/                # the founding paper, the hierarchy, the glossary, the non-goals
```

## Contributing

The contribution guide, the code of conduct, and the issue and pull-request templates live in the organisation profile repository, `.github`. A change that alters the meaning of a term, the shape of the hierarchy, or the boundary of the concept is a change request against `aop-governance`, not a direct edit here.

## Licence

MIT. See `LICENSE`.

# AOP Conceptual Hierarchy: Agentic Operating Engineering, Agentic Operating Procedure, Agent Skill, Domain Agent Harness, Agent, Agentic Operations Levels (Concept Scope)

_The six levels of the concept, the architectural responsibility each one carries, and the principle that holds them together._

| Field | Value |
|---|---|
| Version | 0.1.0 |
| Status | Stable |
| Scope | Concept Scope |
| Owner | Emmanuel A. Otchere |

## 1. The hierarchy

Six levels. Each level names a concept and states the architectural responsibility that concept carries. The ladder descends in scope and ascends in specificity.

| # | Concept | Architectural responsibility |
|---|---|---|
| 1 | Agentic Operating Engineering | The discipline |
| 2 | Agentic Operating Procedure | The operational specification |
| 3 | Agent Skill | The reusable capability |
| 4 | Domain Agent Harness | The controlled execution environment |
| 5 | Agent | The execution actor |
| 6 | Agentic Operations | The broader operating mode |

## 2. Reading the ladder in both directions

Read top to bottom as a discipline: the concept governs how the discipline is practised, the procedure specifies the operating intent, the skill packages the reusable capability, the harness controls the execution environment, the agent acts, and the operating mode is the regime those actions produce.

Read bottom to top as a containment: the operating mode contains agents, agents run inside a harness, a harness is governed by an AOP, an AOP invokes skills, and the whole apparatus is an expression of the discipline.

The two readings are the same ladder. That is the point of it: the concept and the containment structure are not two designs competing to be the real one.

## 3. The governing principle

**The procedure governs the agent, not the other way around.**

The agent operates within the authority, the constraints and the assurance requirements that the AOP establishes. It cannot self-authorise. The authority check is performed by a component outside the model context, so the agent cannot influence the outcome of the check that governs it.

This is the single technical commitment on which the rest of the programme rests. Every other design decision is downstream of it. If a design decision cannot be reconciled with this principle, the design decision is wrong.

## 4. What each level contributes

### 4.1 Agentic Operating Engineering: the discipline

The practice of specifying, implementing, governing and assuring agentic execution. It is a discipline in the sense that it has a method, a body of standards, a way of measuring its own results, and a community that can be wrong in public and be corrected.

The discipline is not AI, and not a platform. It applies to any execution actor that interprets context and acts, whether or not the reasoning is done by a model.

### 4.2 Agentic Operating Procedure: the operational specification

A versioned, machine-readable operating standard that states intent, context, constraints, authority, capabilities, coordination, control and assurance. All eight dimensions are mandatory.

An AOP is network-native in structure: it contains variants, decision points, exception edges and rework loops. A linear procedure is a special case with one variant and no exceptions, and it is precisely the case the concept was built to escape.

### 4.3 Agent Skill: the reusable capability

Atomic, well-scoped, tool-agnostic, composable, independently testable. A skill declares what it does, what it needs, what it must not do, and how it reports. A skill is a capability; it is not authority, and it carries none of its own.

### 4.4 Domain Agent Harness: the controlled execution environment

The top-level AOP for its domain. It sets the boundary conditions under which the agents inside it operate: what may be done, which tools may be called, which credentials may be held, how escalation works, and how the work is verified.

A harness that has not itself been specified as an AOP is not a harness. It is a runtime.

### 4.5 Agent: the execution actor

The agent consumes an AOP, a skill and a context snapshot, and produces actions and evidence. The agent has no authority of its own. Everything it is permitted to do, it is permitted to do because the AOP said so.

### 4.6 Agentic Operations: the broader operating mode

The regime in which agents hold delegated authority over defined operational surface, and humans hold exception ownership rather than corridor execution. The maturity path runs from human-operated, through assisted, to agentic, to autonomous.

## 5. The failure modes the hierarchy addresses

Three failure modes bound the agency of any actor that reads prose.

**Prose semantics.** Natural language admits multiple readings. Two operators reading the same SOP can act differently and both be right. An agent cannot resolve ambiguity at execution time because it has no authority to do so.

**Coverage decay.** The document and the work diverge as soon as either moves, and the gap widens silently because the document is not tested against the work.

**The happy-path fallacy.** The documented path is a minority of real cases. The stated coverage is the coverage of the proposal, not the coverage of the operation.

The hierarchy answers all three with the same move: compile the procedure from observed work rather than authoring it from intent, then govern the agent with what was observed.

## 6. How the levels map to the estate

| Concept | Architectural responsibility | Primary home | Supporting homes |
|---|---|---|---|
| Agentic Operating Engineering | The discipline | `aop-foundations` | `aop-landscape`, `.github` |
| Agentic Operating Procedure | The operational specification | `aop-spec` | `aop-architecture`, `aop-governance` |
| Agent Skill | The reusable capability | `aop-spec` annex | `aop-toolkit`, `aop-registry`, `aop-context-graph` |
| Domain Agent Harness | The controlled execution environment | `aop-reference-harness` | `aop-architecture`, `aop-conformance` |
| Agent | The execution actor | `aop-reference-harness` | `aop-evaluation` |
| Agentic Operations | The broader operating mode | `aop-adoption` | `aop-examples`, `aop-landscape` |

Every repository in the estate resolves to exactly one level, or to an explicitly declared contiguous range of levels.

## 7. Related documents

- [`aop-founding-paper-concept-scope.md`](aop-founding-paper-concept-scope.md): the founding paper.
- [`aop-glossary-concept-scope.md`](aop-glossary-concept-scope.md): the defined terms.
- [`aop-non-goals-concept-scope.md`](aop-non-goals-concept-scope.md): the boundaries of the concept.

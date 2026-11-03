# AOP Glossary: Agentic Operating Engineering, Agentic Operating Procedure, Agent Skill, Domain Agent Harness, Agent, Agentic Operations Levels (Concept Scope)

_Every defined term in the programme, with a stable identifier. A term is defined here once and used consistently everywhere else._

| Field | Value |
|---|---|
| Version | 0.1.0 |
| Status | Stable |
| Scope | Concept Scope |
| Owner | Emmanuel A. Otchere |

Terms are listed in identifier order within their group. The identifier is stable for the life of the term: a term that is renamed keeps its identifier, and a term that is retired keeps its identifier with a shim.

## 1. Core artefacts

| ID | Term | Definition |
|---|---|---|
| AOP-001 | Agentic Operating Procedure | A versioned, machine-readable operational specification that defines how agents may interpret intent, make decisions, coordinate capabilities and execute actions within explicitly governed operational boundaries, to achieve verifiable outcomes. All eight dimensions are mandatory. |
| AOP-002 | Agent Skill | An atomic, well-scoped, tool-agnostic, composable, independently testable unit of capability that an agent can invoke. A skill declares what it does, what it needs, what it must not do, and how it reports. |
| AOP-003 | Domain Agent Harness | The controlled execution environment for a domain. It is the top-level AOP for that domain and defines what agents inside it may do, which tools they may call, which credentials they may hold, how they escalate, and how their work is verified. |
| AOP-004 | Agent | The execution actor. An agent consumes an AOP, a skill and a context snapshot, and produces actions and evidence. An agent holds no authority of its own. |
| AOP-005 | Agentic Operating Engineering | The discipline of specifying, implementing, governing and assuring agentic execution. |

## 2. The eight dimensions

Every AOP populates all eight. The dimension names are fixed; the content is domain-specific.

| ID | Dimension | Definition |
|---|---|---|
| AOP-010 | Intent | The operational objective and desired outcome. |
| AOP-011 | Context | The information and environmental state relevant to execution. |
| AOP-012 | Constraints | Policies, rules, boundaries and prohibited actions. |
| AOP-013 | Authority | The decisions an agent may take alone, and those requiring approval. |
| AOP-014 | Capabilities | The skills, tools and operational capabilities available. |
| AOP-015 | Coordination | How agents, humans and external systems interact. |
| AOP-016 | Control | Monitoring, validation, intervention and exception handling. |
| AOP-017 | Assurance | The evidence required to establish that execution was correct and that outcomes were achieved. |

## 3. Structure of a procedure

| ID | Term | Definition |
|---|---|---|
| AOP-020 | Variant | An observed path through the work, with an observed frequency. The corridor is the rare case. |
| AOP-021 | Decision point | A location in the work where a choice is made, and the rule that governs it. |
| AOP-022 | Exception edge | A location where the work leaves the anticipated path. |
| AOP-023 | Rework loop | A path by which the work returns to an earlier point. |
| AOP-024 | Authority boundary | The set of decisions the agent may take without human approval, and the boundary beyond which it must escalate. |

## 4. Governance and control

| ID | Term | Definition |
|---|---|---|
| AOP-030 | Authority check | The evaluation of an action against the AOP's authority, performed by a component outside the model context so the agent cannot influence the outcome. |
| AOP-031 | Guardrail | The enforcement layer of the harness: permitted-action check, authority-threshold check, exception-pattern check, credential scoping, and escalation dispatch. |
| AOP-032 | Escalation | The transfer of a decision to a human at a defined threshold, with an evidence bundle. |
| AOP-033 | Evidence bundle | The context snapshot, matched variant, applicable rule, proposed action and options, presented to an approver. |
| AOP-034 | Case record | The append-only record of inputs, context snapshot, rule applied, provenance, decision, approver where relevant, and outcome. |
| AOP-035 | Provenance | The chain from a published artefact back to the observed cases and source material it was compiled from. |
| AOP-036 | Drift | The divergence between the current shape of the work and the last known shape. |

## 5. Pipeline

| ID | Term | Definition |
|---|---|---|
| AOP-040 | Observe | The capture of work activity as events, with personal data excluded by default and the capture surface a declared subset of the work surface. |
| AOP-041 | Model | The stitching of events into cases and then into the Context Graph of Work. |
| AOP-042 | Compile | The extraction of variants, decision rules with thresholds, and exception patterns from observed work, with governance bounds and provenance attached, producing a versioned AOP. |
| AOP-043 | Execute | The runtime cycle: context snapshot, variant match, authority check, action, record, emit. |
| AOP-044 | Context Graph of Work | The entity model of observed work, holding cases, tasks, steps, actors, applications, decisions, rules, exceptions, escalations and outcomes. |
| AOP-045 | Case stitching | The reconstruction of individual cases from an event stream. |
| AOP-046 | Variant mining | The extraction of observed paths through the work, with their observed frequencies. |
| AOP-047 | Decision-rule extraction | The derivation of decision rules, with their thresholds, from observed work. |

## 6. Levels of authority

A claim can be checked, or it cannot. The programme distinguishes three burdens of proof.

| ID | Level | Meaning |
|---|---|---|
| AOP-050 | Declared | This is what the programme says AOP means. Verified by internal consistency and reasoning. |
| AOP-051 | Certified | This document conforms to the AOP specification. Verified by machine validation against the schema and the conformance clauses. |
| AOP-052 | Demonstrated | This works, and here is the evidence. Verified by reproduction by a third party from published artefacts. |

An authoritative concept needs all three. A concept with only the first is an opinion. A concept with the first two is a standard. A concept with all three is a discipline other people can build on without asking permission.

## 7. Programme vocabulary

| ID | Term | Definition |
|---|---|---|
| AOP-060 | AOP | The short form of Agentic Operating Procedure. |
| AOP-061 | SOP | Standard Operating Procedure. A procedural specification describing an approved method, authored from intent. |
| AOP-062 | SOP-to-AOP translation | The six-stage procedural engineering process that converts an SOP into an AOP specification. |
| AOP-063 | Shadow mode | An evaluation mode in which an agent's choices are recorded and compared with the choices a human would have made, without the agent acting. |
| AOP-064 | Autonomy disposition | The decision, for each activity in a procedure, whether it stays human-performed, becomes automated, is delegated to an agent, or requires human approval. |
| AOP-065 | Maturity model | The progression from human-operated, through assisted, to agentic, to autonomous operations. |

## 8. Related documents

- [`aop-founding-paper-concept-scope.md`](aop-founding-paper-concept-scope.md): the founding paper.
- [`aop-conceptual-hierarchy-concept-scope.md`](aop-conceptual-hierarchy-concept-scope.md): the conceptual hierarchy.
- [`aop-non-goals-concept-scope.md`](aop-non-goals-concept-scope.md): the non-goals.

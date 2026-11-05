# AOP Hierarchy and Metamodel Map: The Normative Alignment of the Six Levels and the Four Scopes (Concept Scope)

Normative for alignment. This document is CR-010's remainder: the one authoritative mapping between the six-level conceptual hierarchy (the estate's levels) and the staged metamodel's four architectural scopes, closing the last open reconciliation point (point 1's mapping deliverable). Where this document and the metamodel mapping's disposition note differ, this document governs.

## 1. The two structures

The six levels (ratified, `aop-foundations`):

| # | Concept | Architectural responsibility |
|---|---|---|
| 1 | Agentic Operating Engineering | The discipline |
| 2 | Agentic Operating Procedure | The operational specification |
| 3 | Agent Skill | The reusable capability |
| 4 | Domain Agent Harness | The controlled execution environment |
| 5 | Agent | The execution actor |
| 6 | Agentic Operations | The broader operating mode |

The metamodel's four scopes (from the owner's staged documents): Level 1 the metamodel itself, Level 2 AOP specifications, Level 3 operationalisation (domain agent harnesses), Level 4 runtime (AOP executions).

## 2. The normative map

| Metamodel scope | Six-level correspondence | What lives there |
|---|---|---|
| L1 Metamodel | Frames all six levels | The entity register (AOP-E01 to E103) and the specification aspects: the vocabulary every level is described with |
| L2 AOP specifications | Level 2 (the AOP) and level 3 (the Agent Skill, via the contract annex) | The versioned, machine-readable specification artefacts: the AOP document and the skill declarations it may invoke |
| L3 Operationalisation | Level 4 (the Domain Agent Harness), specified as its own top-level AOP per SEC-11 | The execution environment, itself governed by an AOP: what the estate calls a harness is an L3 scope whose boundary document is an L2 artefact |
| L4 Runtime | Level 5 (the Agent) and the run itself | The execution actors and their runs: cases, decisions, records; described by the runtime entities E61 to E75 |

Level 1 (the discipline) and level 6 (the operating mode) are not scopes in the metamodel sense: the discipline is the practice that authors L2 artefacts and operates L3/L4 systems; the operating mode is the regime the runs produce. The metamodel describes artefacts and executions; the hierarchy adds the practice above and the regime below. The two structures are therefore complementary, not competing: the hierarchy answers "what kinds of things exist in agentic operations"; the metamodel answers "how are those things modelled, specified, operationalised and executed".

## 3. The classification rule

HM-1: Any artefact in the estate classifies by asking two questions, in order: (a) is it executed? If no, it is an L2 specification (an AOP or a skill declaration; if it describes the discipline or the regime rather than a governed artefact, it is a foundations or landscape document, outside the metamodel's scopes). (b) If executed: does it act (an agent, L4, level 5) or does it bound acting (a harness, L3, level 4, itself carrying an L2 top-level AOP)? No artefact yields contradictory answers under this rule.

HM-2: The recursion is closed: a harness is a top-level AOP (SEC-11), so a harness-boundary document classifies as L2 while the running harness classifies as L3. This is a composition rule, not a metaphor: the harness AOP is validated like any AOP (the reference harness's own top-level AOP is), and its conformance obligations are the document profile's.

HM-3: Level 6 (Agentic Operations) is reached, not declared: an estate's maturity stage (adoption's model) describes how much of its L3/L4 surface runs under governed L2 artefacts. The regime is the measured state of the estate, which is why the maturity statement cites evidence.

## 4. Disposition

This map settles reconciliation point 1's deliverable (the single normative mapping). The metamodel mapping document in `aop-spec` records the disposition and links here; the source errata note that the earlier open status is superseded.

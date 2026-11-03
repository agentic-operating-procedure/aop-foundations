# AOP Founding Paper: Agentic Operating Engineering, Agentic Operating Procedure, Agent Skill, Domain Agent Harness, Agent, Agentic Operations Levels (Concept Scope)

_What an Agentic Operating Procedure is, where it came from, and why it is a different artefact class from a Standard Operating Procedure._

| Field | Value |
|---|---|
| Version | 0.1.0 |
| Status | Stable |
| Scope | Concept Scope |
| Owner | Emmanuel A. Otchere |

## 1. The question this answers

For decades, Standard Operating Procedures have provided the foundation for operational consistency in enterprises. They document established ways of working, prescribe activities, define responsibilities and establish controls so that operations are performed predictably and in accordance with organisational requirements.

They serve that purpose well where the work can be sufficiently understood, decomposed and prescribed in advance. Their underlying assumption is that the execution path can be defined beforehand and that operational actors, whether human or automated, can follow the prescribed instructions to achieve the intended result.

That assumption becomes restrictive in environments characterised by dynamic conditions, contextual decision-making, distributed intelligence and continuously changing operational requirements.

The emergence of agentic systems introduces a different execution paradigm. Rather than simply following predefined instructions, agents can interpret operational context, reason about available options, select actions, coordinate with other agents and adapt their execution in response to changing circumstances.

So if an agentic system is expected to perform operational work, what replaces the traditional operating procedure as its governing instrument?

The answer proposed here is the Agentic Operating Procedure.

An AOP represents an evolution in procedural engineering. It moves beyond prescribing a fixed sequence of activities towards defining the intent, constraints, decision authority, capabilities, control mechanisms and evidence requirements within which agentic execution is permitted to operate.

It is not an SOP rewritten for an agentic actor. It is a different approach to specifying, governing and assuring operational execution.

## 2. What the traditional procedure does well, and where it stops

A Standard Operating Procedure is a procedural specification. It describes an approved method for carrying out a particular activity or achieving an operational objective. A typical one establishes purpose, scope, roles, preconditions, activities, controls, exceptions and outputs.

The strength of that model is procedural predictability. Its limitation is that it encodes operational knowledge as predefined instructions.

Consider a network incident management procedure. A conventional SOP might prescribe this sequence:

1. Detect an incident.
2. Classify its severity.
3. Notify the responsible team.
4. Investigate the underlying cause.
5. Execute an approved remediation.
6. Verify service restoration.
7. Close the incident.

That is a reasonable procedural specification. But the actual execution depends on the incident's characteristics, the network topology, the affected services, available resources, historical evidence, and the operational impact of potential interventions. A rigid sequence cannot adequately represent every combination of those conditions.

The traditional response is to add decision trees, exception procedures, escalation paths and supplementary instructions. Over time this produces increasingly complex procedural documentation without fundamentally changing the execution model. The complexity is absorbed by the document instead of being resolved by the design.

## 3. What an AOP specifies

An Agentic Operating Procedure is a structured operational specification that defines how agents may interpret intent, make decisions, coordinate capabilities and execute actions within explicitly governed operational boundaries, to achieve verifiable outcomes.

Unlike an SOP, which primarily prescribes activities and their execution sequence, an AOP establishes the conditions under which an agentic system can determine and adapt its execution path.

| Dimension | What the AOP establishes |
|---|---|
| Intent | The operational objective and desired outcome |
| Context | The information and environmental state relevant to execution |
| Constraints | Policies, rules, boundaries and prohibited actions |
| Authority | The decisions an agent may make independently and those requiring approval |
| Capabilities | The skills, tools and operational capabilities available |
| Coordination | How agents, humans and external systems interact |
| Control | Monitoring, validation, intervention and exception handling |
| Assurance | Evidence required to establish that execution was correct and outcomes achieved |

All eight are mandatory. A document that omits one of them is not a degraded AOP; it is not an AOP.

An AOP does not necessarily prescribe every action an agent must take. Instead it specifies what the agent is expected to achieve, what it is permitted to do, what resources it may use, how it should respond to changing conditions, and how its execution will be evaluated.

This introduces a shift from procedural conformity to bounded, evidence-driven execution. The procedure remains authoritative, but the execution path can become adaptive.

## 4. The change in execution paradigm

The relationship between SOPs and AOPs is not a simple replacement. An SOP remains a valuable source of operational knowledge, organisational policy and established controls, and it can provide the foundation from which an AOP is engineered. Translating an SOP into an AOP requires more than converting procedural steps into agent instructions. It requires examining the underlying operational intent, identifying which decisions can be delegated, determining which activities require human intervention, identifying the capabilities needed for execution, and establishing the controls necessary to assure behaviour.

| Dimension | SOP | AOP |
|---|---|---|
| Primary orientation | Prescribed procedure | Governed operational intent |
| Execution model | Predetermined steps | Adaptive execution within boundaries |
| Decision-making | Human-defined decision points | Explicitly delegated decision authority |
| Context | Referenced or predefined | Actively interpreted and used |
| Exceptions | Documented exception paths | Contextual handling within authorised boundaries |
| Capabilities | Tools and resources referenced | Agent-accessible skills, tools and services |
| Coordination | Roles and hand-offs | Dynamic coordination between agents, humans and systems |
| Assurance | Compliance with procedure | Compliance, execution evidence and outcome verification |

An AOP is therefore not inherently autonomous. It may require human approval at every significant decision point, or it may permit substantial independent execution within an approved authority boundary. The degree of autonomy is a separate design consideration.

## 5. The architecture of an AOP

An AOP is understood as part of a broader agentic operating architecture rather than as an isolated instruction document. Four architectural elements matter.

**The AOP specification.** The AOP is the authoritative operational specification. It defines intent, operational context, constraints, decision rights, expected outcomes, control requirements and assurance criteria. It establishes the normative basis against which agent execution is governed.

**Agent Skills.** A skill is a reusable unit of capability that an agent can invoke to perform a particular function: incident classification, root cause analysis, policy evaluation, service configuration, risk assessment, operational reporting. A skill is not an operating procedure. It provides a capability that may be used within one or more procedures. The AOP determines when a capability is appropriate, under what conditions it may be invoked, and what requirements govern its use.

**Domain Agent Harness.** A harness provides the controlled execution environment within which agents operate. It brings together the runtime infrastructure, domain knowledge, tools, interfaces, permissions, policies, observability and execution controls needed to perform operational work. The harness is not the procedure itself; it supplies and enforces the execution capabilities and boundaries required to implement the AOP. An AOP is therefore an important instrument for engineering a domain-specific agent harness, because it provides a structured specification of what the harness must support and enforce.

**Agents and execution instances.** Agents are the execution actors. They interpret the AOP, invoke available capabilities, interact with the operational environment, coordinate with other actors and produce evidence of execution. Individual execution instances are governed by the AOP but are not themselves the AOP. That distinction allows a single AOP to govern multiple agents, execution environments and operational scenarios.

## 6. The relationships between the artefacts

The concepts serve different architectural purposes and should not be conflated.

- The SOP provides procedural source material, not an automatic implementation blueprint.
- The AOP is the governing operational specification.
- Agent Skills provide reusable capabilities.
- The Domain Agent Harness supplies the controlled execution environment.
- Agents perform the work under the AOP's authority and constraints.
- Execution evidence provides the basis for verification, assurance and continuous improvement.

A skill does not implement an SOP step by definition. A skill may support multiple procedures, and an AOP may require several skills to achieve a single outcome. Likewise, an AOP does not become a harness merely because it describes the expected behaviour of agents: the harness must implement and enforce the necessary execution controls.

## 7. AOP as a foundation for domain agent harnesses

One of the more significant implications of AOP is its potential to establish a systematic engineering path towards domain-specific agent harnesses.

Today, agent implementations frequently begin with a model, a collection of tools and a set of instructions. While this can demonstrate useful behaviour, it does not necessarily establish a reliable operational system. A domain-specific harness needs a much stronger foundation. It must understand the domain in which it operates, the operational outcomes it is expected to achieve, the policies it must observe, the decisions it is authorised to make, and the evidence required to demonstrate correct execution.

An AOP provides a structured means of expressing these requirements. Rather than engineering a harness around loosely defined instructions, the engineering process begins with the operational specification and derives the necessary execution architecture from it. This creates a more disciplined relationship between operational requirements, domain knowledge and semantics, agent capabilities, runtime architecture, decision authority, and governance and assurance. The result is a shift from building agents that happen to perform operational tasks, towards engineering governed agentic systems designed to fulfil defined operational responsibilities.

## 8. From SOP to AOP: procedural engineering

The transition from SOP to AOP is an engineering process. Not every SOP should be converted directly, and not every procedural step should become an agent action. A useful transformation approach consists of six stages.

1. **Procedural decomposition.** Examine the existing SOP and identify its underlying intent, activities, decision points, dependencies, controls, exceptions and expected outcomes.
2. **Operational grounding.** Establish the relevant domain semantics, operational context, policies, information requirements and relationships between the entities involved. Agents need more than instructions; they need a grounded understanding of the environment in which those instructions apply.
3. **Autonomy disposition.** Determine which activities remain human-performed, which can be automated, which can be delegated to agents, and which require human approval or supervision. Base the decision on risk, authority, reversibility, operational impact and assurance requirements.
4. **AOP specification.** Construct the AOP by defining its intent, constraints, decision authority, capabilities, coordination requirements, control mechanisms and outcome criteria.
5. **Harness engineering.** Establish the domain agent harness required to execute the AOP, including its skills, tools, knowledge sources, interfaces, permissions, runtime controls and observability.
6. **Verification and assurance.** Validate that the AOP is executable, that the harness enforces its boundaries, that agents operate within their authority, and that the resulting outcomes can be verified through execution evidence.

This process transforms procedural knowledge into an operational specification for governed agentic execution.

## 9. What AOP does not mean

AOP is not synonymous with AI. Agentic execution may use AI, but AI is a technology; AOP is an operational specification.

AOP is not synonymous with automation. Automation executes predefined mechanisms, whereas agentic execution may interpret context and determine an appropriate course of action within its authority.

AOP is not synonymous with autonomy. Agentic describes a mode of operation; autonomous describes the degree of independent execution. An AOP can govern fully supervised, partially autonomous or highly autonomous execution.

AOP is not an Agent Skill. A skill provides a reusable capability; an AOP governs the operational use and coordination of capabilities.

AOP is not an Agent Harness. The AOP defines what must be achieved and the boundaries within which execution occurs; the harness provides the controlled environment that enables and enforces that execution.

These distinctions are essential if AOP is to develop into a coherent engineering discipline rather than another label for AI-assisted workflows. The non-goals are stated in full in [`aop-non-goals-concept-scope.md`](aop-non-goals-concept-scope.md).

## 10. Towards Agentic Operating Engineering

Traditional procedural engineering has largely focused on documenting, standardising and controlling how work is performed. Agentic Operating Engineering extends that discipline to the specification, implementation, governance and assurance of agentic execution. It requires engineers to reason about operational intent, domain semantics, decision authority, capability composition, execution boundaries, dynamic coordination and evidence-based verification.

The objective is not to eliminate procedures, human accountability or operational controls. It is to evolve the way these elements are expressed and implemented, so that both human and non-human actors can participate in operational execution under a common, governed framework.

This also creates a practical migration path. Organisations do not need to discard their existing procedure libraries and start again. They can progressively identify procedures suitable for agentic execution, engineer the corresponding AOP specifications, establish the necessary domain harnesses, and expand agentic participation as the maturity of their governance and assurance mechanisms develops.

The long-term opportunity is a transition from procedural documentation as the primary instrument of operational control, towards executable, semantically grounded and continuously assured operating specifications.

An SOP tells an operational actor how work should be performed. An AOP establishes how an agentic operating system may determine and execute the work, within what authority, under which constraints, and with what evidence of success.

That is the fundamental shift from Standard Operating Procedures to Agentic Operating Procedures.

## References

- [`aop-conceptual-hierarchy-concept-scope.md`](aop-conceptual-hierarchy-concept-scope.md): the six-level conceptual hierarchy this document is indexed by.
- [`aop-glossary-concept-scope.md`](aop-glossary-concept-scope.md): the defined terms used above.

# Q1 — NIST AI RMF 1.0 Core: Within-Framework Synthesis

**Status:** First-pass synthesis; researcher-authored; adversarial and independent review pending  
**Date:** 2026-11-07  
**Protocol:** Q1 Research Protocol v1.0  
**Primary source:** NIST AI 100-1, *Artificial Intelligence Risk Management Framework (AI RMF 1.0)*, January 2023  
**Scope:** Core Functions, Categories, Subcategories, and explanatory text needed to interpret the Core  
**Supporting extraction records:** GOVERN (file 09), MAP (file 10), MEASURE (file 11), MANAGE (file 12)

## 1. Purpose and status

This document synthesizes the four first-pass NIST AI RMF 1.0 Core extraction matrices. It does not add a new coding instrument, rating, ranking, or completeness claim. It organizes already-recorded findings across the ten analytical dimensions approved in Q1 Protocol v1.0 and identifies what the Core does and does not establish for the research question.

This is an investigator-side synthesis. The four extraction matrices have been source-checked against the official public NIST AI 100-1 PDF; independent second-coder review and adversarial review remain pending.

The synthesis does not repeat the historical C1–C20 analysis and does not use those criteria as its analytical instrument.

## 2. Native structure and function-level logic

NIST AI RMF 1.0 Core contains four Functions, 19 Categories, and 72 Subcategories:

| Function | Categories | Subcategories | Primary function-level role |
|---|---:|---:|---|
| GOVERN | 6 | 19 | Establishes organizational governance, accountability, policies, roles, culture, and oversight arrangements that inform the other Functions. |
| MAP | 5 | 18 | Establishes the context for framing AI-system risks, including purposes, requirements, scope, capabilities, affected actors, and impacts. |
| MEASURE | 4 | 22 | Uses quantitative, qualitative, or mixed methods to analyze, assess, benchmark, test, and monitor AI risks and related impacts. |
| MANAGE | 4 | 13 | Prioritizes and treats mapped/measured risks through response, recovery, monitoring, and continual improvement. |
| **Total** | **19** | **72** | **Four interrelated risk-management Functions.** |

The Core is an outcomes-and-actions structure. NIST states that actions are not a checklist and are not necessarily an ordered set of steps. GOVERN is cross-cutting; MAP, MEASURE, and MANAGE can be applied in system-specific contexts and at lifecycle stages. The process is intended to be continuous and iterative.

**Interpretive consequence:** The Core should not be represented as a fixed linear sequence or as a complete engineering workflow specification. Its native structure is a flexible AI risk-management framework organized around Functions, Categories, Subcategories, and associated outcomes/actions.

## 3. Synthesis by approved analytical dimension

### D1 — Stated purpose and intended application

**Explicitly supported in the Core:**
- MAP 1.1 addresses intended purposes, beneficial uses, context-specific laws/norms/expectations, deployment settings, user types, and assumptions/limitations.
- MAP 1.3 and MAP 1.4 address organizational mission/goals and business-use context.
- MAP 3.1 and MAP 3.3 address intended functionality/benefits and targeted application scope.
- MANAGE 1.1 asks whether the AI system achieves its intended purposes and stated objectives and whether development or deployment should proceed.
- MANAGE 2.4 addresses intervention when AI-system performance or outcomes are inconsistent with intended use.

**Bounded interpretation:** NIST explicitly addresses AI-system purpose, intended use, application scope, and consistency with intended objectives. These are relevant to intent-preservation questions at the system/application level.

**Not established by these provisions alone:** a complete representation of an individual human's intent for a particular software-engineering task; a rule for preserving that intent through every intermediate AI-assisted action; or a formal authorization mechanism for changing task intent or engineering scope.

### D2 — Primary object and level of governance

The Core operates across multiple related levels:
- **Organization:** most visible in GOVERN's policies, leadership, roles, accountability, culture, and risk tolerance.
- **AI system and components:** central in MAP's context, categorization, capability, scope, risks, and impacts; MEASURE's testing and monitoring; and MANAGE's risk treatment and system intervention.
- **Lifecycle:** reflected across design, development, deployment, operation, monitoring, evaluation, and decommissioning.
- **Actors and affected parties:** included through role definition, consultation, user input, and community impact.

**Bounded interpretation:** The Core is not exclusively organization-level or system-level; the functions address interrelated organizational and AI-system contexts. However, the explicit units are generally organizational risk-management arrangements and AI systems/components, rather than individual delegated engineering actions.

### D3 — Structural organization and normative/functional character

NIST organizes the Core into four Functions, Categories, and Subcategories. The Core describes outcomes and actions for risk management; it is voluntary and flexible, and the actions are not a checklist or necessarily ordered steps.

**Bounded interpretation:** This is a functional risk-management framework structure, not a clause-based management-system standard structure. Its outcomes can inform organizational processes, but the Core does not itself provide a single mandatory workflow or prescribe one implementation sequence for all users.

### D4 — Organizational governance, leadership, roles, and responsibilities

**Explicitly supported:**
- GOVERN 2.1–2.3 addresses documented roles/responsibilities, training, and executive leadership responsibility for decisions about risks associated with AI-system development and deployment.
- GOVERN 3.2 addresses defining and differentiating roles/responsibilities for human-AI configurations and AI-system oversight.
- MAP 1.2 and MAP 3.4 address relevant actor competencies and operator/practitioner proficiency.
- MAP 3.5 links human-oversight processes to organizational policies established through GOVERN.
- MEASURE 1.3 supports review by internal experts not serving as front-line developers and/or independent assessors, plus relevant consultation.
- MANAGE 2.4 requires assigned and understood responsibilities for superseding, disengaging, or deactivating certain AI systems.

**Bounded interpretation:** Organizational role definition, executive risk responsibility, human-AI role differentiation, operator competence, and selected intervention responsibilities are explicit.

**Not established by these provisions alone:** a complete authority matrix assigning every engineering decision to a named human role; a universal separation-of-duties model for all AI-assisted coding; or a full delegation contract between a human engineer and an AI agent.

### D5 — Human oversight and decision-related provisions

The Core contains several distinct forms of human-related decision and control language. They must not be collapsed into one generic “human approval” category.

| Provision | What the text establishes | What must not be assumed |
|---|---|---|
| GOVERN 2.3 | Executive leadership responsibility for decisions about risks associated with AI-system development and deployment. | Executive approval of every engineering task, code change, or AI output. |
| GOVERN 3.2 | Policies/procedures define and differentiate human-AI roles and AI-system oversight responsibilities. | A complete task-level delegation or approval protocol. |
| MAP 2.2 | Documentation of AI-system knowledge limits and how outputs may be used and overseen by humans, to support decisions and subsequent actions. | Mandatory prior human approval for every output. |
| MAP 3.5 | Human-oversight processes are defined, assessed, and documented in accordance with GOVERN policies. | One prescribed oversight model or approval granularity. |
| MEASURE 2.9 | Model explanation/validation/documentation and contextual interpretation of outputs to inform responsible use and governance. | Guaranteed correctness, full interpretability, or a universal approval event. |
| MEASURE 3.3 | End users and impacted communities can report problems and appeal system outcomes; feedback enters evaluation metrics. | Appeal as equivalent to operator override, pre-implementation approval, or engineering-scope authority. |
| MANAGE 1.1 | A determination is made whether an AI system achieves intended purposes/objectives and whether development or deployment should proceed. | A separate go/no-go approval for every downstream engineering action. |
| MANAGE 2.4 | Assigned responsibilities for superseding, disengaging, or deactivating AI systems inconsistent with intended use. | An unrestricted human override model for all human-AI activities. |
| MANAGE 4.1 | Post-deployment monitoring plans include appeal and override, among other mechanisms. | Defined override actor, trigger, procedure, timing, precedence, or universal applicability. |

**Synthesis:** Human oversight and decision-related provisions are materially present in the Core. The strongest explicit terms include role differentiation, documented oversight processes, system-level proceed/stop decisions, assigned system-disengagement responsibilities, and post-deployment appeal/override mechanisms.

**Remaining specification gap in the examined Core text:** These provisions do not, taken together, define a complete task-level authorization model for AI-assisted engineering. In particular, the exact authority holder, delegation boundaries, approval granularity, pre-implementation gate, change-of-intent procedure, and technical enforcement semantics are not comprehensively specified by the cited Subcategories.

This is a bounded statement about what the examined Core establishes; it is not a claim that NIST has no additional relevant guidance outside the Core or in other publications.

### D6 — AI risk identification, analysis, evaluation, and treatment

Risk management is the central subject of all four Functions:
- GOVERN establishes policies, accountability, organizational risk culture, third-party governance, and risk-management arrangements.
- MAP identifies context, requirements, system capabilities, scope, components, potential benefits, costs, and impacts.
- MEASURE selects metrics, conducts testing and evaluation, assesses trustworthiness, tracks risks, and examines measurement effectiveness.
- MANAGE prioritizes and treats risks, documents residual risks, responds to incidents, and improves controls.

**Bounded interpretation:** The Core has extensive and explicit coverage of AI risk-management activities. This coverage should not be translated into a claim that it defines every form of engineering authority or every decision-rights question.

### D7 — Lifecycle processes, monitoring, change, and continual improvement

Lifecycle references are distributed throughout the Core:
- GOVERN covers organizational practices across design, development, deployment, evaluation, use, monitoring, and decommissioning.
- MAP considers purposes, assumptions, deployment contexts, components, and impacts as they evolve.
- MEASURE includes pre-deployment testing, production monitoring, regular risk tracking, and field-context evaluation.
- MANAGE addresses response, recovery, post-deployment monitoring, change management, decommissioning, and continual improvement.

**Bounded interpretation:** Lifecycle coverage is explicit and broad. Change management is explicitly named in MANAGE 4.1, and continual improvement is explicit in MANAGE 4.2. Neither statement alone establishes a complete approval-before-implementation workflow for every software or configuration change.

### D8 — Documentation, records, measurement, evaluation, and evidence

Documentation and measurement are distributed rather than confined to one Function:
- GOVERN includes documented policies, roles, processes, risks, impacts, and review arrangements.
- MAP documents intended purposes, assumptions, requirements, system scope, knowledge limits, oversight arrangements, risks, and impacts.
- MEASURE documents test sets, metrics, tools, results, uncertainty, evaluations, and risk tracking.
- MANAGE documents risk treatment, residual risks, response/recovery, incident processes, and continual-improvement activities.

**Bounded interpretation:** The Core explicitly expects documentation and records across risk-management activities and uses measurement results to inform management decisions.

**Not established by these provisions alone:** a single mandatory evidence schema, universal provenance format, complete decision-log structure, or end-to-end traceability model for every AI-assisted engineering action. Documentation requirements should not be overstated as proof that a specific record is sufficient for a specific authorization claim.

### D9 — Implementation, assessment, and assurance mechanisms

The Core supports implementation through organizational policies/processes, human-oversight processes, risk inventories, testing, TEVV, metrics, independent review processes, production monitoring, appeals, overrides, incident response, recovery, and continual improvement.

**Bounded interpretation:** NIST provides multiple implementation and assessment mechanisms. The function-level discussion of MEASURE includes rigorous software testing, uncertainty, benchmark comparison, formal reporting, and independent review processes. These provisions support assessment and assurance-related activity.

**Not established by these provisions alone:** certification, conformity assessment, a universal audit procedure, or proof that following the Core makes a particular AI system safe or an organization compliant with all applicable obligations.

### D10 — Source-access and interpretation limits

For NIST AI RMF 1.0, the full public NIST AI 100-1 PDF was available and examined. The four extraction matrices record native locations and first-pass interpretations for all 72 Core Subcategories.

Limits remain:
- The extraction is researcher-authored and not yet independently second-coded.
- The analysis is limited to NIST AI RMF 1.0 and does not silently substitute a later edition or revision.
- The AI RMF Playbook, profiles as separate implementation resources, and other NIST publications were not treated as primary evidence in this Core extraction.
- Presence of a Subcategory does not establish organizational implementation or effectiveness.
- The NIST 1.0 revision-status qualification recorded in the Q1 source register remains applicable.

## 4. Cross-function relationships

The Core's internal logic is interdependent rather than four separate checklists:

1. **GOVERN supplies organizational direction and accountability.** It establishes policies, roles, and processes that inform the other Functions.
2. **MAP supplies context.** It identifies the purposes, intended uses, requirements, scope, actors, capabilities, components, and impacts needed to frame risks.
3. **MEASURE evaluates.** It uses mapped risks and context to test, assess, benchmark, and monitor system behavior and trustworthiness.
4. **MANAGE responds.** It uses mapped and measured information to prioritize risk treatment, respond, recover, monitor, and improve.

The source describes this work as continuous and iterative. The functions may be applied flexibly according to user needs and capacities, while governance remains cross-cutting.

## 5. What the examined NIST Core establishes — and does not establish

### Established by explicit source provisions

- Organizational AI-risk governance, accountability, roles, and executive risk responsibility.
- Differentiation of human-AI roles and responsibilities for oversight.
- Contextual documentation of intended purposes, system requirements, application scope, and knowledge limits.
- Defined, assessed, and documented human-oversight processes.
- Risk measurement, software testing, TEVV, uncertainty, benchmarking, and documented evaluation.
- Production monitoring, incident reporting/response/recovery, and continual improvement.
- System-level decisions about whether development/deployment should proceed.
- Assigned responsibilities for superseding, disengaging, or deactivating certain AI systems.
- Post-deployment monitoring plans that include appeal and override mechanisms.

### Not established as a complete model by the examined Core provisions

- A complete task-level authorization model for AI-assisted engineering.
- A universal requirement for human approval before every AI-generated code change or engineering action.
- A complete delegation contract specifying permitted actions, limits, escalation, and revocation for an AI agent acting within a software project.
- A fully specified mechanism for preserving an individual human's task intent through all intermediate engineering actions.
- Exact operational semantics for the actor, trigger, timing, precedence, and enforcement of every appeal/override mechanism.
- A universal evidence/provenance schema or complete end-to-end engineering traceability format.

“Not established as a complete model” is not equivalent to “absent from every NIST publication” or “not addressed at all.” It describes the limits of the examined Core evidence and the scope of this analysis.

## 6. Counterevidence and alternative readings that must be retained

A balanced synthesis must not minimize the following explicit NIST provisions:
- MAP 2.2 and MAP 3.5 directly address human use/oversight and defined/assessed/documented oversight processes.
- MANAGE 1.1 explicitly requires a determination about whether development or deployment should proceed.
- MANAGE 1.3 explicitly includes acceptance among risk-treatment options.
- MANAGE 2.4 explicitly assigns responsibilities for superseding, disengaging, or deactivating systems inconsistent with intended use.
- MANAGE 4.1 explicitly names appeal and override as elements of post-deployment monitoring plans.

These provisions are substantive and relevant. The limitation is not that NIST says nothing about human control or decisions; the limitation is that the examined Core does not fully specify their task-level authority semantics for AI-assisted engineering.

## 7. Provisional NIST-only conclusion

NIST AI RMF 1.0 Core provides a structured, flexible, lifecycle-oriented approach to organizational AI risk management. It contains explicit provisions on organizational accountability, human-AI role differentiation, human oversight, intended use and application scope, measurement and evidence, system-level proceed/stop decisions, system disengagement, appeal, and override.

The Core therefore provides meaningful source-grounded coverage of several governance and human-control topics relevant to this research. However, the examined provisions do not, as a complete set, establish a fully specified task-level authorization and delegation model for AI-assisted engineering, nor a universal approval-before-implementation requirement for each engineering action.

This conclusion is limited to the NIST AI RMF 1.0 Core and the source material examined. It is not a judgment of NIST's overall adequacy, implementation effectiveness, or comparative standing against ISO/IEC 42001 or BAES.

## 8. Review questions for adversarial examination

The following questions should be used to challenge this synthesis before cross-framework comparison:

1. Does the synthesis understate or overstate the significance of MANAGE 4.1's explicit “appeal and override” language?
2. Is MANAGE 1.1 correctly characterized as a system-level development/deployment decision, rather than a universal per-action approval gate?
3. Does MANAGE 2.4 establish an operationally meaningful intervention responsibility, and have its limits been described without discounting its significance?
4. Are MAP 2.2 and MAP 3.5 correctly distinguished as human-use/oversight documentation and oversight-process provisions, rather than full authorization semantics?
5. Is the distinction between organizational risk acceptance and task-level engineering authorization sufficiently precise?
6. Are there any explicit Core statements that materially contradict the “complete task-level authorization model not established” conclusion?
7. Are any dimension mappings in files 09–12 over-coded, under-coded, or inconsistent with the approved ten-dimension definitions?
8. Does the synthesis preserve the difference between source statements, researcher interpretations, and unknowns?

## 9. Verification and review status

| Item | Status |
|---|---|
| Four native Function matrices completed | Yes — 19 / 18 / 22 / 13 Subcategories |
| Total native Subcategory count | 72; all identifiers unique in the four extraction records |
| Source edition | NIST AI 100-1 / AI RMF 1.0, January 2023 |
| Primary source-location checks | Completed by researcher for the four Core tables and relevant function-level explanations |
| Historical C1–C20 used as coding instrument | No |
| Within-NIST synthesis | First pass complete |
| Adversarial review | Pending |
| Independent second-coder review | Pending |
| Cross-framework comparison | Not updated by this document |
| BAES repository changes | None |

## 10. Sources and linked records

- NIST AI 100-1, *Artificial Intelligence Risk Management Framework (AI RMF 1.0)*, January 2023. [Official PDF](https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.100-1.pdf).
- [09 — GOVERN extraction matrix](09-Q1-NIST-Core-Extraction-Matrix-GOVERN.md).
- [10 — MAP extraction matrix](10-Q1-NIST-Core-Extraction-Matrix-MAP.md).
- [11 — MEASURE extraction matrix](11-Q1-NIST-Core-Extraction-Matrix-MEASURE.md).
- [12 — MANAGE extraction matrix](12-Q1-NIST-Core-Extraction-Matrix-MANAGE.md).
- [02 — Q1 Research Protocol v1.0](02-Q1-Research-Protocol-v1.0.md).

---

**Control note:** This synthesis is a first-pass NIST-only analysis. Do not update the comparative memo or make external claims until adversarial review, source rechecks, and the ISO public-preview work have been completed to the extent feasible.

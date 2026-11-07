# Q1 — NIST AI RMF 1.0 Core Extraction Matrix: MANAGE

**Status:** First-pass analytical extraction; researcher source-checked; independent review pending  
**Date:** 2026-11-07  
**Protocol:** Q1 Research Protocol v1.0  
**Source ID:** Q1-NIST-001  
**Primary source:** [NIST AI 100-1, AI RMF 1.0 (PDF)](https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.100-1.pdf)  
**Native source location:** Part 2, Section 5.4, Table 4, printed pp. 32–33 (PDF pages 36–37)

## 1. Purpose and method

This file records the fourth NIST Core extraction tranche: all 13 MANAGE Subcategories. Each item is mapped to the ten analytical dimensions approved in Q1 Research Protocol v1.0, retaining NIST's native Function / Category / Subcategory structure.

This is a researcher-authored first-pass analysis, not a NIST classification, score, ranking, completeness claim, or independent validation. Source statements are paraphrased; dimension assignments and bounded notes are researcher judgments. The historical C1–C20 criteria are not used as the sampling frame or coding instrument.

MANAGE allocates resources to mapped and measured risks and includes response, recovery, communication, monitoring, and continual improvement. Several Subcategories contain especially relevant decision or control language: determining whether development/deployment should proceed (MANAGE 1.1), assigning responsibilities to supersede/disengage/deactivate systems (MANAGE 2.4), and post-deployment monitoring including appeal and override (MANAGE 4.1). Their scope and specificity must be stated accurately; they do not automatically establish a complete task-level authorization model for AI-assisted engineering.

## 2. Analytical dimension key

| Code | Approved Q1 dimension |
|---|---|
| D1 | Stated purpose and intended application |
| D2 | Primary object and level of governance (organization, AI system, lifecycle, process, or other source-defined unit) |
| D3 | Structural organization and normative/functional character |
| D4 | Organizational governance, leadership, roles, and responsibilities |
| D5 | Human oversight and decision-related provisions |
| D6 | AI risk identification, analysis, evaluation, and treatment |
| D7 | Lifecycle processes, monitoring, change, and continual improvement |
| D8 | Documentation, records, measurement, evaluation, and evidence |
| D9 | Implementation, assessment, and assurance mechanisms explicitly supported by the examined source |
| D10 | Source-access and interpretation limits |

D10 is applied where a limitation materially qualifies interpretation; it is not automatically assigned to every Subcategory.

## 3. Evidence-status and mapping conventions

- **Explicit:** the Subcategory's source wording directly addresses the mapped dimension.
- **Indirect:** the dimension is relevant through context or a reasonable, bounded interpretation, but is not directly stated as the Subcategory's subject.
- **Not established:** the examined text does not establish the proposition being tested. This is not equivalent to absence from the full framework.
- **Access-limited:** the necessary source text was not available for examination.
- **Not applicable:** the dimension does not apply to the source unit under analysis.

The complete public NIST AI RMF 1.0 PDF was examined. Table 4 and the surrounding Section 5.4 discussion were checked at the printed pages identified above. Dimension assignments and interpretations remain researcher judgments.

## 4. MANAGE extraction — 13 Subcategories

| Native ID | Source page | Native category / source-level subject (paraphrase) | Q1 dimensions | Evidence status | Bounded analytical note |
|---|---:|---|---|---|---|
| MANAGE 1.1 | 32 | A determination is made whether the AI system achieves its intended purposes and stated objectives and whether its development or deployment should proceed. | D1, D2, D5, D6, D9 | Explicit | Direct system-level proceed/stop decision tied to intended purpose and objectives. The Subcategory does not identify the decision-maker or specify approval authority for every subsequent engineering task or change. |
| MANAGE 1.2 | 32 | Treatment of documented AI risks is prioritized based on impact, likelihood, and available resources or methods. | D6, D7, D8, D9 | Explicit | Direct risk-treatment prioritization. It does not itself allocate decision rights for each treatment action. |
| MANAGE 1.3 | 32 | Responses to high-priority AI risks are developed, planned, and documented; options include mitigating, transferring, avoiding, or accepting risk. | D6, D7, D8, D9 | Explicit | Explicitly names risk acceptance as one response option. This does not, by itself, define who is authorized to accept which risk, at what threshold, or under what delegation. |
| MANAGE 1.4 | 32 | Negative residual risks to downstream acquirers and end users are documented. | D2, D6, D8 | Explicit | Direct residual-risk documentation provision. Documentation alone does not establish that a risk has been approved or accepted by an authorized person. |
| MANAGE 2.1 | 32 | Resources required for risk management are considered alongside viable non-AI alternatives to reduce potential impact magnitude or likelihood. | D1, D2, D6, D9 | Explicit | Connects risk treatment to resources and non-AI alternatives. It does not prescribe a specific approval or procurement authority. |
| MANAGE 2.2 | 32 | Mechanisms are in place and applied to sustain the value of deployed AI systems. | D2, D7, D9 | Explicit | A broad operational-sustainment outcome. The Subcategory does not specify a particular mechanism or decision-rights structure. |
| MANAGE 2.3 | 32 | Procedures are followed to respond to and recover from a previously unknown risk when identified. | D6, D7, D9 | Explicit | Direct response/recovery procedure for newly identified risk. Detailed escalation authority and approval thresholds are not specified here. |
| MANAGE 2.4 | 32 | Mechanisms are applied, and responsibilities are assigned and understood, to supersede, disengage, or deactivate AI systems whose performance or outcomes conflict with intended use. | D1, D4, D5, D7, D9 | Explicit | Direct responsibility assignment for consequential system-level intervention, including disengagement/deactivation. It does not define the specific responsible role, trigger thresholds, or whether this is equivalent to a general human override over all AI-assisted engineering actions. |
| MANAGE 3.1 | 32 | Risks and benefits from third-party resources are regularly monitored, with risk controls applied and documented. | D2, D6, D7, D8, D9 | Explicit | Direct third-party risk monitoring/control provision. It does not specify authority for every supplier or component change. |
| MANAGE 3.2 | 32 | Pre-trained models used in development are included in regular AI-system monitoring and maintenance. | D2, D6, D7, D9 | Explicit | Extends monitoring to pre-trained models used in development. It does not define a model-specific authorization or change-approval process. |
| MANAGE 4.1 | 33 | Post-deployment monitoring plans are implemented, including mechanisms for user/actor input, appeal and override, decommissioning, incident response, recovery, and change management. | D2, D4, D5, D6, D7, D8, D9 | Explicit | The clearest direct reference to appeal and override in the Core table. It establishes these as elements of post-deployment monitoring plans but does not specify the authorized human role, exact override mechanics, precedence, timing, or applicability to each AI-assisted engineering action. |
| MANAGE 4.2 | 33 | Measurable continual-improvement activities are integrated into AI-system updates and include regular engagement with interested parties and relevant AI actors. | D4, D6, D7, D8, D9 | Explicit | Direct continual-improvement and update provision with stakeholder engagement. It does not equate consultation with approval or specify a change authorization workflow. |
| MANAGE 4.3 | 33 | Incidents and errors are communicated to relevant actors, including affected communities; tracking, response, and recovery processes are followed and documented. | D4, D6, D7, D8, D9 | Explicit | Direct incident communication, tracking, response, recovery, and documentation. Detailed incident command and decision rights are not fully specified in this Subcategory. |

## 5. First-tranche observations

These observations are limited to MANAGE. Together with the separate GOVERN, MAP, and MEASURE matrices, they complete the first-pass extraction of all four NIST AI RMF 1.0 Core Functions.

1. **MANAGE contains explicit system-level proceed/stop language.** MANAGE 1.1 calls for determining whether an AI system achieves its intended purposes/objectives and whether development or deployment should proceed. This is more direct decision language than the MAP context-setting provisions, but the stated object remains the AI system's development/deployment.
2. **Risk acceptance is an explicit response option.** MANAGE 1.3 names mitigating, transferring, avoiding, and accepting high-priority AI risks. The Subcategory does not itself identify who may accept risk, define approval thresholds, or provide a complete delegation matrix.
3. **Responsibility for system disengagement is explicit.** MANAGE 2.4 requires responsibilities to be assigned and understood for superseding, disengaging, or deactivating AI systems with performance/outcomes inconsistent with intended use. This is a consequential system-level intervention provision; its exact role and trigger mechanics are not specified in the Subcategory.
4. **Appeal and override are explicitly named.** MANAGE 4.1 includes appeal and override among mechanisms within post-deployment monitoring plans. This is an important direct source finding and must not be omitted from synthesis. However, the text does not define the precise override actor, procedure, scope, timing, or technical enforcement.
5. **Change management and continual improvement are included.** MANAGE 4.1 addresses change management; MANAGE 4.2 integrates measurable continual improvement into AI-system updates. Neither statement alone specifies a complete human authorization gate for every engineering change.
6. **Response and recovery are lifecycle activities.** MANAGE 2.3 and 4.3 address newly identified risks, incidents, errors, response, recovery, communication, and documentation.
7. **MANAGE uses prior functions' outputs.** The function-level explanation links risk treatment to information from MAP and MEASURE and governance arrangements from GOVERN. The Core should therefore be interpreted as an interrelated risk-management structure, not as four isolated checklists.
8. **No inference about implementation effectiveness follows.** The presence of these outcomes in the Core does not establish that a particular organization has implemented them or that the mechanisms are effective in practice.

## 6. Specific authority- and control-related cautions

The following distinctions must remain intact in subsequent synthesis:

- **System development/deployment proceed decision** (MANAGE 1.1) is not automatically approval authority for each downstream engineering task, code change, or AI-generated output.
- **Risk acceptance as a treatment option** (MANAGE 1.3) is not a complete specification of the authorized risk acceptor, delegation boundaries, or acceptance thresholds.
- **Assigned responsibility to disengage/deactivate an AI system** (MANAGE 2.4) is not automatically a general human override model for all human-AI work.
- **Appeal and override** (MANAGE 4.1) are explicit source terms, but their exact operational semantics and applicability must not be invented.
- **Change management and continual improvement** (MANAGE 4.1–4.2) are not automatically equivalent to explicit approval-before-implementation for every change.
- **Incident response/recovery responsibility** is not the same as ordinary authorization for planned engineering work.

These are limits on what the cited MANAGE text establishes, not claims that no related provisions exist elsewhere in NIST AI RMF 1.0.

## 7. Verification record

| Check | Result |
|---|---|
| Native structure retained | 4 MANAGE Categories / 13 MANAGE Subcategories |
| Source table location checked | NIST AI 100-1, Table 4, printed pp. 32–33 |
| Surrounding MANAGE explanation checked | Section 5.4, printed pp. 31–32 |
| Subcategory identifiers checked against inventory | 13 identifiers represented |
| Source wording | Paraphrased; no extended quotation |
| Dimension assignments | Researcher first-pass judgment |
| Independent second-coder review | Pending |
| Historical C1–C20 criteria used as coding instrument | No |
| Claims about implementation/effectiveness | None |
| Task-level authorization conclusion | No universal task-level authorization requirement inferred |

## 8. Sources

- NIST AI 100-1, *Artificial Intelligence Risk Management Framework (AI RMF 1.0)*, January 2023, Part 2, Section 5.4, Table 4, printed pp. 32–33. [Official PDF](https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.100-1.pdf).
- NIST AI 100-1, Part 2, Section 5.4, explanatory text on risk treatment, response, recovery, monitoring, and continual improvement, printed pp. 31–32.
- Q1 Protocol v1.0, Sections 5–8, for the ten analytical dimensions and interpretation constraints.

## 9. Next stage

The first-pass source extraction of all 72 NIST AI RMF 1.0 Core Subcategories is now complete across GOVERN, MAP, MEASURE, and MANAGE. Next: perform a within-NIST synthesis, check dimension-level coverage and cross-function relationships, then conduct adversarial review before updating the cross-framework comparison. Independent second-coder review remains pending.

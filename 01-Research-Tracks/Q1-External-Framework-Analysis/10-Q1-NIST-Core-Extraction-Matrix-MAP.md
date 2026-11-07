# Q1 — NIST AI RMF 1.0 Core Extraction Matrix: MAP

**Status:** First-pass analytical extraction; researcher source-checked; independent review pending  
**Date:** 2026-11-07  
**Protocol:** Q1 Research Protocol v1.0  
**Source ID:** Q1-NIST-001  
**Primary source:** [NIST AI 100-1, AI RMF 1.0 (PDF)](https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.100-1.pdf)  
**Native source location:** Part 2, Section 5.2, Table 2, printed pp. 26–28 (PDF pages 30–32)

## 1. Purpose and method

This file records the second NIST Core extraction tranche: all 18 MAP Subcategories. It maps each item to the ten analytical dimensions approved in Q1 Protocol v1.0, preserving NIST's native Function / Category / Subcategory structure.

The mapping is a researcher-authored first-pass analysis, not a NIST classification, score, ranking, completeness claim, or independent validation. Source statements are paraphrased; dimension assignments and bounded notes are researcher judgments. The historical C1–C20 criteria are not used as the sampling frame or coding instrument.

MAP establishes context for framing AI-system risks. NIST explains that information gathered through MAP informs risk prevention, model-management decisions, and an initial decision about whether an AI solution is appropriate or whether design, development, or deployment should proceed. This initial system-level go/no-go function must not be silently reinterpreted as a universal approval gate for each AI-assisted engineering action or code change.

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

For this tranche, the complete public NIST AI RMF 1.0 PDF is available. The MAP table and surrounding explanatory text were checked at the printed pages identified above. Dimension assignments and interpretations remain researcher judgments.

## 4. MAP extraction — 18 Subcategories

| Native ID | Source page | Native category / source-level subject (paraphrase) | Q1 dimensions | Evidence status | Bounded analytical note |
|---|---:|---|---|---|---|
| MAP 1.1 | 26 | Intended purposes, beneficial uses, laws, norms, expectations, deployment settings, user types and expectations, potential impacts, assumptions, limitations, and relevant TEVV/metrics are understood and documented. | D1, D2, D6, D8 | Explicit | Strong context- and purpose-documentation provision. It establishes a basis for understanding intended use and risk; it does not itself establish a human authorization protocol for later changes to that purpose. |
| MAP 1.2 | 26 | Interdisciplinary AI actors' competencies, skills, capacities, demographic diversity, domain/user experience, and participation are reflected and documented; collaboration is prioritized. | D4, D8, D9 | Explicit | Addresses who contributes to context establishment and the documentation of participation. It does not allocate final decision authority or establish an approval hierarchy. |
| MAP 1.3 | 26 | The organization's mission and relevant goals for AI technology are understood and documented. | D1, D2, D4, D8 | Explicit | The object is organizational mission and AI-related goals. This is relevant to purpose alignment but does not define an individual user's task-level intent or a change-authorization rule. |
| MAP 1.4 | 26 | Business value or the business-use context is clearly defined, or re-evaluated for an existing AI system. | D1, D2, D8 | Explicit | Defines/reassesses business-use context. It should not be treated as a complete specification of user intent, engineering requirements, or delegated agent permissions. |
| MAP 1.5 | 26 | Organizational risk tolerances are determined and documented. | D2, D4, D6, D8 | Explicit | Directly concerns organizational risk tolerance. NIST's broader discussion says the Framework does not prescribe risk tolerance; this Subcategory requires it to be determined and documented by the organization. |
| MAP 1.6 | 26 | System requirements are elicited from and understood by relevant AI actors; design decisions account for socio-technical implications to address AI risks. | D2, D4, D6, D8, D9 | Explicit | Explicit requirements elicitation and socio-technical design consideration. The text does not specify a formal requirements-baseline authority, change-control workflow, or rule that an AI system may not alter requirements without task-specific human approval. |
| MAP 2.1 | 26 | The specific tasks the AI system will support and the methods used to implement those tasks are defined. | D2, D3, D8 | Explicit | Defines the AI system's supported tasks and implementation methods. This is system categorization, not by itself a delegation contract assigning permitted actions to an AI agent in a software project. |
| MAP 2.2 | 26 | Information about AI-system knowledge limits and how outputs may be used and overseen by humans is documented, with sufficient information to support relevant actors' decisions and subsequent actions. | D2, D5, D8, D9 | Explicit | Directly addresses documentation of knowledge limits, human use/oversight of outputs, and decision support. It does not specify the exact approval authority, required approval event, or universal human sign-off for every output. |
| MAP 2.3 | 27 | Scientific integrity and TEVV considerations—including experimental design, data collection/selection, system trustworthiness, and construct validation—are identified and documented. | D6, D8, D9 | Explicit | Directly supports documented scientific and evaluation considerations. It is not a general authorization or delegation provision. |
| MAP 3.1 | 27 | Potential benefits of intended AI-system functionality and performance are examined and documented. | D1, D6, D8 | Explicit | Evaluates benefits against intended functionality. The intended-functionality framing is relevant to purpose, but does not independently define authority to revise that purpose. |
| MAP 3.2 | 27 | Potential costs, including non-monetary costs from expected or realized errors, functionality, and trustworthiness, are examined and documented in relation to organizational risk tolerance. | D2, D6, D8 | Explicit | Risk/cost analysis is linked to organizational tolerance. It does not establish who may accept a particular residual risk in every operational decision; other governance provisions may be relevant. |
| MAP 3.3 | 27 | Targeted application scope is specified and documented based on capability, established context, and AI-system categorization. | D1, D2, D3, D8 | Explicit | Explicit system application-scope definition. This is relevant to scope boundaries, but the Subcategory does not specify a task-level change authorization mechanism or enforcement control for an AI agent. |
| MAP 3.4 | 27 | Processes for operator and practitioner proficiency regarding AI-system performance/trustworthiness and relevant standards/certifications are defined, assessed, and documented. | D4, D8, D9 | Explicit | Addresses operator/practitioner competence and its assessment. Competence is not equivalent to decision authority, delegation, or approval. |
| MAP 3.5 | 27 | Human-oversight processes are defined, assessed, and documented in accordance with organizational policies established through GOVERN. | D4, D5, D8, D9 | Explicit | Direct human-oversight provision, explicitly linked to organizational governance policies. The source does not, in this Subcategory, prescribe a single oversight model, approval granularity, or task-level authorization semantics. |
| MAP 4.1 | 27 | Approaches for mapping AI-technology and legal risks of all system components, including third-party data/software and rights-infringement risks, are established, followed, and documented. | D2, D6, D7, D8, D9 | Explicit | Extends risk mapping to system components and third-party dependencies. It does not itself define who may authorize a particular engineering change involving those components. |
| MAP 4.2 | 27 | Internal risk controls for AI-system components, including third-party AI technologies, are identified and documented. | D2, D6, D8, D9 | Explicit | Explicit identification/documentation of component-level internal risk controls. The Subcategory does not specify the controls' exact technical form or the authority required to modify them. |
| MAP 5.1 | 27 | Likelihood and magnitude of beneficial and harmful impacts are identified and documented using expected use, analogous prior uses, incident reports, external feedback, or other data. | D2, D6, D8, D9 | Explicit | Direct impact characterization and evidence inputs. It does not establish a universal threshold for accepting impacts or the identity of the final decision-maker for every use context. |
| MAP 5.2 | 28 | Practices and personnel support regular engagement with relevant AI actors and documented integration of feedback about positive, negative, and unanticipated impacts. | D4, D6, D8, D9 | Explicit | Addresses engagement capacity and feedback integration. Unlike GOVERN 5.2, this wording does not itself use the term “adjudicated”; avoid importing that qualifier into MAP 5.2. It is not a general agent-authorization mechanism. |

## 5. First-tranche observations

These observations are limited to MAP and must not be generalized to the complete NIST Core before MEASURE and MANAGE are extracted.

1. **Context and intended purpose are central.** MAP 1.1–1.4 explicitly address intended purposes, organizational mission/goals, business-use context, assumptions, deployment settings, and expectations.
2. **Requirements and application scope are addressed.** MAP 1.6 requires system requirements to be elicited from and understood by relevant AI actors; MAP 3.3 requires targeted application scope to be specified and documented. Neither Subcategory, on its own, supplies a complete task-level authorization or change-control model.
3. **Human oversight is explicit in two particularly direct places.** MAP 2.2 addresses documentation of how AI outputs may be used and overseen by humans; MAP 3.5 requires human-oversight processes to be defined, assessed, and documented in accordance with GOVERN policies.
4. **The oversight provisions are process- and system-contextual.** The text supports documented oversight arrangements and decision-support information. It does not specify a universal approval granularity, a required human approval event for every AI output, or a complete delegation semantics.
5. **MAP includes an initial system-level go/no-go decision.** The surrounding section says contextual knowledge should inform an initial decision about whether to design, develop, or deploy an AI system. This is materially relevant decision language, but its stated object is the appropriateness of the AI system/solution—not every subsequent engineering task or code change.
6. **Risk and impact characterization are documented.** MAP 3.1–3.2 and MAP 5.1 address benefits, costs, likelihood, magnitude, and impact evidence; MAP 4.1–4.2 extend risk mapping to system components and internal controls.
7. **The MAP function is not a complete evidence or assurance regime by itself.** It supplies contextual inputs and documented outputs that inform MEASURE and MANAGE. The Core's functions are iterative and interrelated.
8. **No inference about implementation effectiveness follows.** The existence of these outcomes in the Core does not establish that a particular organization has implemented them or that they work effectively in practice.

## 6. Specific authorization- and intent-related cautions

The following distinctions must remain intact in subsequent synthesis:

- **Intended purpose and system scope** (MAP 1.1, MAP 3.3) are not automatically a complete model of an individual human's intent for a specific engineering task.
- **Requirements elicitation** (MAP 1.6) is not automatically a formal approval-before-implementation or requirements-change authorization rule.
- **Defining supported tasks and methods** (MAP 2.1) is not automatically an agent-specific delegation contract.
- **Documenting human use and oversight of AI outputs** (MAP 2.2) is not automatically proof that every output requires prior human approval.
- **Defining and assessing human-oversight processes** (MAP 3.5) is not automatically a complete task-level authority model.
- **Initial go/no-go about designing, developing, or deploying an AI system** (MAP section 5.2 explanatory text) is not automatically a go/no-go gate for each downstream engineering action.
- **Feedback engagement and integration** (MAP 5.2) is not automatically authorization to change system scope, requirements, or behavior.

These are limits on what the cited MAP text establishes, not claims that no related provisions exist elsewhere in NIST AI RMF 1.0.

## 7. Verification record

| Check | Result |
|---|---|
| Native structure retained | 5 MAP Categories / 18 MAP Subcategories |
| Source table location checked | NIST AI 100-1, Table 2, printed pp. 26–27 |
| Surrounding MAP explanation checked | Section 5.2, printed pp. 24–25 |
| Subcategory identifiers checked against inventory | 18 identifiers represented |
| Source wording | Paraphrased; no extended quotation |
| Dimension assignments | Researcher first-pass judgment |
| Independent second-coder review | Pending |
| Historical C1–C20 criteria used as coding instrument | No |
| Claims about implementation/effectiveness | None |
| Task-level authorization conclusion | No universal task-level authorization requirement inferred |

## 8. Sources

- NIST AI 100-1, *Artificial Intelligence Risk Management Framework (AI RMF 1.0)*, January 2023, Part 2, Section 5.2, Table 2, printed pp. 26–27. [Official PDF](https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.100-1.pdf).
- NIST AI 100-1, Part 2, Section 5.2, explanatory text on MAP's purpose, context, risk information, and initial go/no-go decision, printed pp. 24–25.
- Q1 Protocol v1.0, Sections 5–8, for the ten analytical dimensions and interpretation constraints.

## 9. Next tranche

Continue with **MEASURE (22 Subcategories)** using the same extraction fields, source-location checks, and interpretation safeguards. Do not revise GOVERN or MAP assignments merely to make later cross-framework comparison appear more symmetrical.

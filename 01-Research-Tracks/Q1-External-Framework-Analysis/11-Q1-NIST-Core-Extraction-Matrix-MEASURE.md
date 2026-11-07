# Q1 — NIST AI RMF 1.0 Core Extraction Matrix: MEASURE

**Status:** First-pass analytical extraction; researcher source-checked; independent review pending  
**Date:** 2026-11-07  
**Protocol:** Q1 Research Protocol v1.0  
**Source ID:** Q1-NIST-001  
**Primary source:** [NIST AI 100-1, AI RMF 1.0 (PDF)](https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.100-1.pdf)  
**Native source location:** Part 2, Section 5.3, Table 3, printed pp. 29–31 (PDF pages 33–35)

## 1. Purpose and method

This file records the third NIST Core extraction tranche: all 22 MEASURE Subcategories. Each item is mapped to the ten analytical dimensions approved in Q1 Research Protocol v1.0, retaining NIST's native Function / Category / Subcategory structure.

This is a researcher-authored first-pass analysis, not a NIST classification, score, ranking, completeness claim, or independent validation. Source statements are paraphrased; dimension assignments and bounded notes are researcher judgments. The historical C1–C20 criteria are not used as the sampling frame or coding instrument.

MEASURE uses quantitative, qualitative, or mixed-method approaches to analyze, assess, benchmark, and monitor AI risk and related impacts. Its results inform MANAGE. NIST's surrounding discussion expressly includes software testing, uncertainty, benchmarks, formal reporting, independent review, and measurement of human-AI configurations. These are measurement/evaluation provisions; they must not automatically be recast as a task-level authorization or approval model.

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

The complete public NIST AI RMF 1.0 PDF was examined. Table 3 and the surrounding Section 5.3 discussion were checked at the printed pages identified above. Dimension assignments and interpretations remain researcher judgments.

## 4. MEASURE extraction — 22 Subcategories

| Native ID | Source page | Native category / source-level subject (paraphrase) | Q1 dimensions | Evidence status | Bounded analytical note |
|---|---:|---|---|---|---|
| MEASURE 1.1 | 29 | Measurement approaches and metrics for MAP-identified AI risks are selected, beginning with the most significant risks; risks or trustworthiness characteristics that cannot or will not be measured are documented. | D6, D8, D9 | Explicit | Directly addresses risk measurement selection and documentation of measurement gaps. It does not imply that every risk can be quantified or that a missing metric means no risk exists. |
| MEASURE 1.2 | 29 | Appropriateness of AI metrics and effectiveness of existing controls are regularly assessed and updated, including error reports and potential impacts on affected communities. | D6, D7, D8, D9 | Explicit | Supports recurring evaluation of metrics and controls. It does not define the authority required to approve every control change. |
| MEASURE 1.3 | 29 | Internal experts not serving as front-line developers and/or independent assessors participate in regular assessments and updates; relevant experts, users, external actors, and affected communities are consulted as appropriate to risk tolerance. | D4, D6, D8, D9 | Explicit | Provides for review separated from front-line development and consultation. It does not make every assessment formally independent, nor does it allocate final decision authority. |
| MEASURE 2.1 | 29 | Test sets, metrics, and details of tools used during TEVV are documented. | D6, D8, D9 | Explicit | Direct evidence/documentation provision for evaluation inputs and tools. No common evidence schema or universal traceability format is prescribed in this Subcategory. |
| MEASURE 2.2 | 29 | Evaluations involving human subjects meet applicable requirements, including human-subject protection, and are representative of the relevant population. | D2, D6, D9 | Explicit | Concerns protection and representativeness in evaluations involving human subjects. It should not be misclassified as a human oversight or engineering-approval provision. |
| MEASURE 2.3 | 29 | AI-system performance or assurance criteria are measured qualitatively or quantitatively and demonstrated under conditions similar to deployment; measures are documented. | D2, D6, D8, D9 | Explicit | Direct performance/assurance measurement under deployment-like conditions. “Assurance criteria” here do not, without more, establish authorization criteria for individual engineering actions. |
| MEASURE 2.4 | 29 | Functionality and behavior of the AI system and its components, as identified in MAP, are monitored in production. | D2, D6, D7, D9 | Explicit | Direct production-monitoring provision. The object is AI-system functionality and behavior, not necessarily every AI-assisted engineering action or repository change. |
| MEASURE 2.5 | 29 | The AI system to be deployed is demonstrated to be valid and reliable; limits on generalizability beyond development conditions are documented. | D2, D6, D8, D9 | Explicit | Addresses validity, reliability, and generalizability limits. Demonstrating system validity does not establish human approval of every later use or modification. |
| MEASURE 2.6 | 30 | The AI system is regularly evaluated for safety risks; deployment requires demonstrated safety, residual negative risk within tolerance, and safe failure, with relevant safety metrics. | D2, D6, D7, D8, D9 | Explicit | Strong system-level safety evaluation and residual-risk provision. It does not specify a universal task-level approval workflow or identify one decision-maker for every engineering change. |
| MEASURE 2.7 | 30 | AI-system security and resilience risks identified through MAP are evaluated and documented. | D2, D6, D8, D9 | Explicit | Direct security/resilience evaluation and documentation. It does not define the full operational authorization structure for changes to controls. |
| MEASURE 2.8 | 30 | Risks associated with transparency and accountability, as identified in MAP, are examined and documented. | D4, D6, D8, D9 | Explicit | Evaluates transparency/accountability risks. The Subcategory does not itself define specific accountable roles or an approval mechanism. |
| MEASURE 2.9 | 30 | The AI model is explained, validated, and documented; system output is interpreted in context to inform responsible use and governance. | D2, D5, D6, D8, D9 | Explicit | Supports contextual interpretation of outputs for responsible use and governance. This is not equivalent to a guarantee that outputs are understandable, correct, or subject to prior human approval in every instance. |
| MEASURE 2.10 | 30 | AI-system privacy risk identified through MAP is examined and documented. | D2, D6, D8, D9 | Explicit | Direct privacy-risk examination and documentation; no specific authorization model is stated. |
| MEASURE 2.11 | 30 | Fairness and bias identified through MAP are evaluated and results documented. | D2, D6, D8, D9 | Explicit | Direct evaluation/documentation of fairness and bias. It does not specify who has final authority over every resulting mitigation decision. |
| MEASURE 2.12 | 30 | Environmental impact and sustainability of AI-model training and management activities are assessed and documented. | D2, D6, D7, D8, D9 | Explicit | Addresses environmental and sustainability impacts of training/management activities. It is a system/activity impact measure, not a human-authority provision. |
| MEASURE 2.13 | 30 | Effectiveness of the TEVV metrics and processes used in MEASURE is evaluated and documented. | D6, D7, D8, D9 | Explicit | Evaluates the evaluation system itself. This supports methodological review, not a specific delegation or approval model. |
| MEASURE 3.1 | 30 | Approaches, personnel, and documentation support regular identification and tracking of existing, unanticipated, and emergent AI risks, including in deployed contexts. | D4, D6, D7, D8, D9 | Explicit | Direct risk-tracking provision with personnel and documentation. It does not establish a complete incident decision-rights matrix. |
| MEASURE 3.2 | 30 | Risk-tracking approaches are considered where risks are difficult to assess using available techniques or where metrics do not yet exist. | D6, D7, D8 | Explicit | Recognizes measurement limitations and the need for risk tracking despite unavailable metrics. Absence of a metric is not evidence of absence of risk. |
| MEASURE 3.3 | 31 | Feedback processes allow end users and impacted communities to report problems and appeal system outcomes; feedback is integrated into AI-system evaluation metrics. | D2, D5, D6, D8, D9 | Explicit | Explicitly addresses reporting and appeal of AI-system outcomes. Appeal is not automatically the same as operator override, pre-deployment approval, or authority to change engineering scope. |
| MEASURE 4.1 | 31 | Measurement approaches are linked to deployment contexts and informed by consultation with domain experts and end users; approaches are documented. | D2, D4, D6, D8, D9 | Explicit | Contextualizes measurement and consultation. Consultation does not by itself allocate decision authority to consultees. |
| MEASURE 4.2 | 31 | Trustworthiness measurement results across deployment contexts and the AI lifecycle are informed by relevant expert/actor input to validate whether performance is consistent with intended behavior; results are documented. | D1, D4, D6, D7, D8, D9 | Explicit | Explicitly tests consistency with intended performance using input and documented results. It does not itself define who may amend intended behavior or approve a deviation. |
| MEASURE 4.3 | 31 | Measurable performance improvements or declines are identified and documented using consultations with relevant actors, affected communities, and field data about context-relevant risks and trustworthiness. | D4, D6, D7, D8, D9 | Explicit | Supports field-informed change/performance observation and documentation. It does not specify a change-authorization gate or establish that consultation equals approval. |

## 5. First-tranche observations

These observations are limited to MEASURE and must not be generalized to the complete NIST Core before MANAGE is extracted.

1. **Measurement is broader than numeric metrics.** NIST permits quantitative, qualitative, or mixed-method approaches and explicitly recognizes cases where risks or trustworthiness characteristics cannot or will not be measured.
2. **Software testing and uncertainty are explicit in the function-level discussion.** The surrounding text calls for rigorous software testing, performance assessment, uncertainty measures, benchmark comparison, formalized reporting, and documentation.
3. **Independent review is supported, but not universally mandated.** NIST says independent review processes can improve testing and mitigate internal bias/conflicts. MEASURE 1.3 provides for internal experts who were not front-line developers and/or independent assessors, with consultation as appropriate. This should not be overstated as a mandatory independent audit for every AI system.
4. **Human-AI configurations are part of measurement.** The function-level discussion expressly includes tracking metrics for human-AI configurations. MEASURE 2.9 and 3.3 add contextual output interpretation and appeal/reporting processes.
5. **Appeal is explicit; its exact authority mechanics are not.** MEASURE 3.3 establishes processes for users and impacted communities to report problems and appeal system outcomes. It does not specify the appeal adjudicator, required remedy, response time, or equivalence to a human override control.
6. **Monitoring extends into deployment.** MEASURE 2.4 and 3.1 address production behavior and ongoing risk tracking; MEASURE 4.2–4.3 connect results to lifecycle context, actor input, and field data.
7. **Measurement supports management decisions but does not itself decide them.** The surrounding text describes measurement as a traceable basis to inform management decisions; MANAGE is the function that uses measurement outcomes for risk response and monitoring.
8. **No inference about implementation effectiveness follows.** The presence of these outcomes in the Core does not establish that an organization has implemented them or that its measurement practices are effective.

## 6. Specific authority- and evidence-related cautions

The following distinctions must remain intact in subsequent synthesis:

- **Independent review as a beneficial process** is not automatically a mandatory independent audit for every system.
- **Assurance/performance criteria** (MEASURE 2.3) are not automatically task-level authorization criteria.
- **Contextual interpretation of AI output** (MEASURE 2.9) is not automatically a requirement for prior human approval of each output.
- **User/community appeal** (MEASURE 3.3) is not automatically equivalent to operator override, human veto, or engineering-change approval.
- **Measurement results informing management decisions** is not the same as the measurement function itself holding decision authority.
- **Observed improvement/decline** (MEASURE 4.3) is not itself permission to modify intended behavior or scope.

These are limits on what the cited MEASURE text establishes, not claims that no related provisions exist elsewhere in NIST AI RMF 1.0.

## 7. Verification record

| Check | Result |
|---|---|
| Native structure retained | 4 MEASURE Categories / 22 MEASURE Subcategories |
| Source table location checked | NIST AI 100-1, Table 3, printed pp. 29–31 |
| Surrounding MEASURE explanation checked | Section 5.3, printed pp. 28–29 |
| Subcategory identifiers checked against inventory | 22 identifiers represented |
| Source wording | Paraphrased; no extended quotation |
| Dimension assignments | Researcher first-pass judgment |
| Independent second-coder review | Pending |
| Historical C1–C20 criteria used as coding instrument | No |
| Claims about implementation/effectiveness | None |
| Task-level authorization conclusion | No universal task-level authorization requirement inferred |

## 8. Sources

- NIST AI 100-1, *Artificial Intelligence Risk Management Framework (AI RMF 1.0)*, January 2023, Part 2, Section 5.3, Table 3, printed pp. 29–31. [Official PDF](https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.100-1.pdf).
- NIST AI 100-1, Part 2, Section 5.3, explanatory text on measurement methods, software testing, uncertainty, independent review, traceability, and monitoring, printed pp. 28–29.
- Q1 Protocol v1.0, Sections 5–8, for the ten analytical dimensions and interpretation constraints.

## 9. Next tranche

Continue with **MANAGE (13 Subcategories)** using the same extraction fields, source-location checks, and interpretation safeguards. After MANAGE, complete a within-NIST synthesis and adversarial review before updating the cross-framework comparison.

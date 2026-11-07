# Q1 — NIST AI RMF 1.0 Core Extraction Matrix: GOVERN

**Status:** First-pass analytical extraction; researcher source-checked; independent review pending  
**Date:** 2026-11-07  
**Protocol:** Q1 Research Protocol v1.0  
**Source ID:** Q1-NIST-001  
**Primary source:** [NIST AI 100-1, AI RMF 1.0 (PDF)](https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.100-1.pdf)  
**Native source location:** Part 2, Section 5.1, Table 1, printed pp. 22–24 (PDF pages 26–28)

## 1. Purpose and method

This file records the first analytical tranche of the NIST Core extraction: all 19 GOVERN Subcategories. It maps each item to the ten dimensions approved in Q1 Protocol v1.0, using NIST's own native Function / Category / Subcategory structure.

This is a researcher-authored analytical mapping, not a NIST classification, score, ranking, completeness claim, or independent validation. The mapping is based on the source text and its surrounding GOVERN discussion. A dimension code means that the source item materially informs that dimension; it does not imply that the source fully specifies the subject.

The historical C1–C20 criteria are not used as the sampling frame or coding instrument.

## 2. Analytical dimension key

| Code | Approved Q1 dimension |
|---|---|
| D1 | Stated purpose and intended application |
| D2 | Primary object and level of governance |
| D3 | Structural organization and normative/functional character |
| D4 | Organizational governance, leadership, roles, and responsibilities |
| D5 | Human oversight and decision-related provisions |
| D6 | AI risk identification, analysis, evaluation, and treatment |
| D7 | Lifecycle processes, monitoring, change, and continual improvement |
| D8 | Documentation, records, measurement, evaluation, and evidence |
| D9 | Implementation, assessment, and assurance mechanisms explicitly supported by the examined source |
| D10 | Source-access and interpretation limits |

D10 is applied at the level of the extraction record where a limitation materially qualifies interpretation. It is not automatically assigned to every Subcategory.

## 3. Evidence-status and mapping conventions

- **Explicit:** the Subcategory's source wording directly addresses the mapped dimension.
- **Indirect:** the dimension is relevant through context or a reasonable, bounded interpretation, but is not directly stated as the Subcategory's subject.
- **Not established:** the examined text does not establish the proposition being tested. This is not equivalent to absence from the full framework.
- **Access-limited:** the necessary source text was not available for examination.
- **Not applicable:** the dimension does not apply to the source unit under analysis.

For this tranche, the source is the complete public NIST AI RMF 1.0 PDF. Each row records the Subcategory's source page and a concise paraphrase. The dimension assignment and interpretation are researcher judgments.

## 4. GOVERN extraction — 19 Subcategories

| Native ID | Source page | Source-level subject (paraphrase) | Q1 dimensions | Evidence status | Bounded analytical note |
|---|---:|---|---|---|---|
| GOVERN 1.1 | 22 | AI-related legal and regulatory requirements are understood, managed, and documented. | D4, D6, D8 | Explicit | Organizational compliance and documentation are explicit. This does not itself define who may authorize an individual engineering action. |
| GOVERN 1.2 | 22 | Trustworthy-AI characteristics are integrated into organizational policies, processes, procedures, and practices. | D4, D6, D9 | Explicit | Establishes organizational integration of trustworthiness considerations; does not prescribe a single operational approval workflow. |
| GOVERN 1.3 | 22 | Organizational processes determine the level of risk-management activity according to organizational risk tolerance. | D4, D6 | Explicit | Risk-management intensity is tied to organizational risk tolerance. NIST separately states that the Framework does not prescribe risk tolerance. |
| GOVERN 1.4 | 22 | Transparent risk-management processes and outcomes are established through policies, procedures, and controls based on organizational risk priorities. | D4, D6, D8, D9 | Explicit | Direct support for policy/control-based risk governance and transparency; no task-level authorization rule is stated here. |
| GOVERN 1.5 | 23 | Ongoing monitoring and periodic review of risk-management processes and outcomes are planned; organizational roles, responsibilities, and review frequency are defined. | D4, D7, D8 | Explicit | Directly addresses governance responsibility and recurring review. The object is the organizational risk-management process and its outcomes. |
| GOVERN 1.6 | 23 | AI systems are inventoried and resourced according to organizational risk priorities. | D2, D4, D6, D8 | Explicit | Establishes an organizational AI-system inventory and risk-prioritized resourcing; it is not an inventory of individual AI-assisted engineering actions. |
| GOVERN 1.7 | 23 | Safe decommissioning and phase-out processes for AI systems are established to avoid increasing risk or reducing trustworthiness. | D6, D7, D9 | Explicit | Lifecycle control at AI-system level. It should not be generalized into a general-purpose human override or engineering-change approval requirement. |
| GOVERN 2.1 | 23 | Roles, responsibilities, and communication lines for AI risk mapping, measurement, and management are documented and clear across the organization. | D4, D8 | Explicit | Direct organizational role/accountability provision, with documentation and communication. It does not specify every role boundary in every human-AI task configuration. |
| GOVERN 2.2 | 23 | Personnel and partners receive AI risk-management training to perform duties consistently with policies, procedures, and agreements. | D4, D9 | Explicit | Addresses capability and preparation to perform assigned risk-management duties; training is not equivalent to authorization. |
| GOVERN 2.3 | 23 | Executive leadership takes responsibility for decisions about risks associated with AI-system development and deployment. | D4, D5, D6 | Explicit | Direct executive-level responsibility for AI-system risk decisions. The text does not establish that executives must approve each engineering task, code change, or AI-generated output. |
| GOVERN 3.1 | 23 | Lifecycle risk-management decisions are informed by teams with diverse demographic, disciplinary, experiential, and expertise backgrounds. | D4, D7, D9 | Explicit | Specifies a team-composition input to risk decisions; it does not itself allocate final decision authority. |
| GOVERN 3.2 | 23 | Policies and procedures define and differentiate roles and responsibilities for human-AI configurations and AI-system oversight. | D4, D5, D9 | Explicit | Direct human-AI role differentiation and oversight provision. The Subcategory does not, by itself, define task-level approval thresholds or delegation semantics. |
| GOVERN 4.1 | 23 | Organizational policies and practices foster critical thinking and a safety-first mindset across AI-system design, development, deployment, and use. | D4, D7, D9 | Explicit | Organizational culture and practice provision across lifecycle stages; it is not a specified review or authorization gate. |
| GOVERN 4.2 | 24 | Teams document risks and potential impacts of AI technologies they design, develop, deploy, evaluate, and use, and communicate impacts more broadly. | D4, D6, D7, D8 | Explicit | Directly supports documentation and communication of risk/impact across lifecycle activities. |
| GOVERN 4.3 | 24 | Organizational practices enable AI testing, incident identification, and information sharing. | D4, D7, D8, D9 | Explicit | Supports testing and incident-information practices. The Subcategory does not prescribe a particular evidence schema or traceability format. |
| GOVERN 5.1 | 24 | Organizational policies and practices collect, consider, prioritize, and integrate external feedback about potential individual and societal impacts of AI risks. | D4, D6, D8, D9 | Explicit | Addresses engagement and feedback integration as part of risk governance. It does not mean all external feedback is automatically accepted. |
| GOVERN 5.2 | 24 | Mechanisms enable teams to incorporate adjudicated feedback from relevant AI actors into system design and implementation on a regular basis. | D4, D7, D9 | Explicit | Feedback is described as adjudicated before incorporation. This is not a general authorization model for AI agents or delegated engineering execution. |
| GOVERN 6.1 | 24 | Policies and procedures address AI risks associated with third parties, including intellectual-property and other rights infringement. | D4, D6, D9 | Explicit | Organizational and supply-chain risk control. It is not a direct human-authority provision. |
| GOVERN 6.2 | 24 | Contingency processes address high-risk failures or incidents in third-party data or AI systems. | D6, D7, D9 | Explicit | Addresses contingency preparedness for third-party failure/incident scenarios; detailed response authority is not specified in this Subcategory. |

## 5. First-tranche observations

These observations are limited to GOVERN and should not be generalized to the complete NIST Core before MAP, MEASURE, and MANAGE have been extracted.

1. **Organizational level is dominant.** GOVERN's Subcategories principally concern organizational policies, processes, accountability structures, leadership, teams, and third-party governance.
2. **Human-AI oversight is explicit but bounded.** GOVERN 3.2 explicitly calls for differentiated roles and responsibilities for human-AI configurations and AI-system oversight. It does not, in its own wording, specify a complete task-level authorization or approval-before-implementation model.
3. **Executive responsibility has a defined object.** GOVERN 2.3 assigns executive leadership responsibility for decisions about risks associated with AI-system development and deployment. It should not be restated as approval authority over every individual engineering action.
4. **Documentation is distributed through governance.** GOVERN 1.1, 1.4, 1.5, 2.1, and 4.2 explicitly include documentation-related outcomes. Other Subcategories establish processes or practices without specifying a common record format.
5. **Lifecycle coverage is present.** GOVERN provisions refer to design, development, deployment, evaluation, use, monitoring, periodic review, and decommissioning. The exact operational implications differ by Subcategory.
6. **The function is cross-cutting.** NIST's surrounding text describes GOVERN as informing and being infused throughout MAP, MEASURE, and MANAGE. This is a structural property of the framework, not an additional Subcategory.
7. **No inference about implementation effectiveness follows.** The existence of these outcomes in the Core does not establish that an organization has implemented them or that they are effective in practice.

## 6. Specific authorization-related caution

The following distinctions must remain intact in subsequent synthesis:

- **Risk decision responsibility** (GOVERN 2.3) is not automatically **authority to approve every engineering change**.
- **Differentiated human-AI roles and oversight** (GOVERN 3.2) is not automatically a complete **delegation model**.
- **Critical-thinking and safety-first culture** (GOVERN 4.1) is not automatically an enforceable **pre-implementation approval gate**.
- **Adjudicated feedback incorporation** (GOVERN 5.2) is not automatically an agent's authority to modify system behavior or project scope.

These are limits on what the cited text establishes, not claims that NIST lacks all related provisions elsewhere in the framework.

## 7. Verification record

| Check | Result |
|---|---|
| Native structure retained | 6 GOVERN Categories / 19 GOVERN Subcategories |
| Source table location checked | NIST AI 100-1, Table 1, printed pp. 22–23 |
| Subcategory identifiers checked against inventory | 19 identifiers represented |
| Source wording | Paraphrased; no extended quotation |
| Dimension assignments | Researcher first-pass judgment |
| Independent second-coder review | Pending |
| Historical C1–C20 criteria used as coding instrument | No |
| Claims about implementation/effectiveness | None |

## 8. Sources

- NIST AI 100-1, *Artificial Intelligence Risk Management Framework (AI RMF 1.0)*, January 2023, Part 2, Section 5.1, Table 1, printed pp. 22–23. [Official PDF](https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.100-1.pdf).
- NIST AI RMF 1.0, Part 2 introductory text on the Core and iterative use, printed pp. 20–21.
- Q1 Protocol v1.0, Sections 5–8, for the ten analytical dimensions and interpretation constraints.

## 9. Next tranche

Continue with **MAP (18 Subcategories)** using the same extraction fields and safeguards. Do not revise the GOVERN assignments merely to make later cross-framework comparison appear more symmetrical.

# Q1 — External Framework Analysis Protocol

**Status:** Approved for research execution  
**Version:** 1.0  
**Approval date:** 2026-11-07  
**Track:** Q1 — External Framework Analysis  
**Supersedes:** Draft v0.1 (retained as historical record)

## 1. Purpose

Conduct a bounded, source-transparent analysis of the native structures and stated purposes of NIST AI RMF 1.0 and ISO/IEC 42001:2023. Establish what can responsibly be said about organizational AI governance, AI risk management, human authority and oversight, evidence/documentation, and lifecycle control from the materials actually examined.

This is a framework analysis, not a ranking, conformity assessment, certification assessment, or evaluation of BAES effectiveness.

## 2. Research question

How do the native structures, stated purposes, and publicly examinable materials of NIST AI RMF 1.0 and ISO/IEC 42001:2023 differ in the way they frame organizational AI governance and AI risk management, and what—if anything—can be responsibly inferred about human authority, oversight, evidence, and lifecycle control from those materials without treating the frameworks as equivalent or claiming access to unavailable ISO clauses?

### Subquestions

- **RQ1.1 — Purpose and object:** What problem, organizational/system object, and intended users does each framework or standard describe?
- **RQ1.2 — Structure:** How does each source organize its content, and what is the appropriate native unit of analysis?
- **RQ1.3 — Governance and responsibility:** What publicly examinable material addresses organizational roles, responsibilities, leadership, oversight, and decision authority?
- **RQ1.4 — Risk and lifecycle:** How are risk identification, assessment, treatment, monitoring, change, and continual improvement represented?
- **RQ1.5 — Evidence and documentation:** What can be established about documented information, records, measurement, evaluation, and traceability from the examined materials?
- **RQ1.6 — Limits:** Which comparisons are defensible, which are non-equivalent, and which remain unknown because source access is incomplete?

## 3. Scope and source boundary

### 3.1 NIST AI RMF

Primary subject: **NIST AI Risk Management Framework (AI RMF 1.0), NIST AI 100-1 (January 2023).**

Primary unit of analysis:
- Functions;
- Categories;
- Subcategories;
- explanatory text necessary to interpret those units.

The four Functions—GOVERN, MAP, MEASURE, and MANAGE—are analyzed in their native structure. Categories and Subcategories remain attached to their native parent functions.

The primary source is the AI RMF 1.0 publication and its Core. The Playbook, profiles published separately, crosswalks, implementation resources, companion publications, and subsequent NIST publications are outside the primary analysis unless a scope extension is recorded in the Decision Register before use.

**Version-status qualification:** NIST's public AI RMF resource page, checked on 2026-11-07, states that AI RMF 1.0 is being updated and that a revised version is in progress. Q1 nevertheless treats AI RMF 1.0 as a fixed historical edition for a reproducible comparison with ISO/IEC 42001:2023. This study must not describe 1.0 as necessarily the latest NIST position at the time of publication. Any later NIST edition or revision is out of scope unless a separately approved protocol amendment is made.

### 3.2 ISO/IEC 42001

Primary subject: **ISO/IEC 42001:2023, Information technology — Artificial intelligence — Management system.**

Permitted materials:
- official ISO and IEC publication/product records;
- official publicly accessible preview material;
- official public descriptions of scope and purpose;
- credible secondary sources, explicitly labelled as secondary and used only for contextual interpretation.

The complete final-edition normative text is not assumed to be available. No clause-level coverage rating, detailed clause reconstruction, or clause-by-clause completeness claim is permitted unless sufficient authorized access to the exact final edition is later established and a protocol amendment is approved.

An FDIS-era crosswalk may be used only as a lead-finding or contextual secondary source. It is not evidence of exact final-edition clause content and is not a normative ISO mapping.

### 3.3 Excluded material

No confidential BAES material, private project material, non-public correspondence, or material from BAES-SECRET may be used. No confidential BAES specification may be inferred from public layer names, labels, or adjacent concepts.

## 4. Prior-work treatment and non-duplication

The following existing work is not repeated:
- historical C1–C20 mapping of NIST AI RMF 1.0 Core;
- public BAES text mapping against the recovered historical criteria;
- S01 Axis B evidence-sufficiency coding;
- Axis C residual ambiguity register;
- prior calibration and comparative scope reviews.

These records are cited as prior project work with their original scope and limitations. The recovered C1–C20 criteria are not Q1's sampling frame or primary analytical instrument.

The [Prior-Work Gap and Overlap Matrix](00-Prior-Work-Gap-Overlap-Matrix.md) is the controlling non-duplication record.

## 5. Approved analytical dimensions

1. Stated purpose and intended application.
2. Primary object and level of governance (organization, AI system, lifecycle, process, or other source-defined unit).
3. Structural organization and normative/functional character.
4. Organizational governance, leadership, roles, and responsibilities.
5. Human oversight and decision-related provisions.
6. AI risk identification, analysis, evaluation, and treatment.
7. Lifecycle processes, monitoring, change, and continual improvement.
8. Documentation, records, measurement, evaluation, and evidence.
9. Implementation, assessment, and assurance mechanisms explicitly supported by the examined source.
10. Source-access and interpretation limits.

A dimension need not be present in both sources or expressed at the same level. Use “not applicable to this source unit” or “not established from examined material” where appropriate.

## 6. Extraction record

For each extracted statement or structural element, record:

| Field | Description |
|---|---|
| Record ID | Stable identifier |
| Framework | NIST AI RMF 1.0 or ISO/IEC 42001:2023 |
| Source ID | Program source-register entry |
| Source type | Primary official / official supporting / secondary |
| Edition and version | Exact version examined |
| Native location | Function/category/subcategory or publicly visible ISO location |
| Analytical dimension | One or more dimensions from Section 5 |
| Source statement | Concise paraphrase; quote only when necessary and permitted |
| Evidence status | Explicit / indirect / not established / access-limited / not applicable |
| Interpretation | Researcher interpretation, separated from source statement |
| Limitation | Scope or access constraint |
| Verification | Self-checked / independently reviewed / pending |

Paraphrases must not be presented as quotations. Quotations must be brief, accurate, attributed, and compliant with source licensing and copyright conditions.

## 7. Analysis procedure

1. Verify source identity, edition, publication status, and access date.
2. Maintain the source register before substantive extraction.
3. Analyze NIST within its own native structure, from Functions through Categories and Subcategories.
4. Analyze ISO only to the depth supported by authorized public material; unavailable normative content remains unknown/access-limited.
5. Complete within-framework descriptions before cross-framework comparison.
6. Compare only dimensions that are sufficiently comparable; explicitly state differences in purpose, unit, and structure.
7. Record counterevidence, ambiguity, and alternative interpretations.
8. Verify every substantive claim against its source location.
9. Produce a limitations-first synthesis.

## 8. Interpretation rules

- A framework's stated purpose does not establish implementation by any particular organization.
- A governance outcome is not automatically a task-level authorization requirement.
- Oversight is not automatically equivalent to explicit approval of a particular engineering change.
- Documentation is not automatically sufficient evidence for a claim.
- A management-system standard and a risk-management framework are not assumed to be equivalent.
- A secondary crosswalk does not override the source's own text.
- Unavailable text is not evidence of absence.
- Conceptual similarity is not proof of equivalence.
- The existence of a topic in a framework does not establish effectiveness.
- A term shared by NIST and BAES, including “Profile”, does not establish equivalent meaning or function.

## 9. Reporting requirements

The report must include:
- research question and scope;
- source register and exact access boundaries;
- native-structure descriptions;
- within-framework findings;
- dimension-by-dimension comparison where defensible;
- counterevidence and interpretive uncertainty;
- explicit unknowns and access limitations;
- deviations from protocol;
- bounded conclusion and limitations.

No composite score, weighted total, ranking, conformity claim, or BAES superiority claim will be produced.

## 10. Validation

At minimum:
- source and citation verification by the researcher;
- adversarial review of interpretations and non-equivalence claims;
- independent reviewer/second-coder review if feasible and separately arranged.

If no independent reviewer participates, the report must identify the analysis as investigator-side and exploratory. Self-review is not independent validation.

## 11. Stop conditions

Pause Q1 and seek Founder direction if:
- a necessary source is not lawfully accessible;
- a proposed comparison requires reconstructing unavailable ISO clauses;
- analysis duplicates the historical C1–C20 work;
- a source or method change materially alters the research question;
- confidential BAES or private project content would be needed;
- an external party requests control over criteria, analysis, findings, or publication.

## 12. Approval and change control

The Founder approved Q1 execution and this protocol's scope on 2026-11-07. Q1 is approved to begin within the boundaries above.

Any material change to the research question, source boundary, analytical dimensions, extraction rules, validation plan, or reporting method must be recorded in the Decision Register before implementation. Approval to execute Q1 does not authorize publication of a final conclusion or modification of any other repository.

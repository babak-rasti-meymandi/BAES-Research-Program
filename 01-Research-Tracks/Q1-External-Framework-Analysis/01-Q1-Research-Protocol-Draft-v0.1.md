# Q1 — External Framework Analysis Protocol (Draft)

**Status:** Draft for Founder review; not approved for substantive analysis.  
**Version:** 0.1  
**Prepared:** 2026-11-07  
**Track:** Q1 — External Framework Analysis

## 1. Purpose

Conduct a bounded, source-transparent analysis of the native structures and stated purposes of NIST AI RMF 1.0 and ISO/IEC 42001:2023. The analysis will identify what can be responsibly said about organizational AI governance, AI risk management, human authority and oversight, evidence/documentation, and lifecycle control from the materials actually examined.

This is a framework analysis, not a framework ranking, conformity assessment, or evaluation of BAES effectiveness.

## 2. Research question

How do the native structures, stated purposes, and publicly examinable materials of NIST AI RMF 1.0 and ISO/IEC 42001:2023 differ in the way they frame organizational AI governance and AI risk management, and what—if anything—can be responsibly inferred about human authority, oversight, evidence, and lifecycle control from those materials without treating the frameworks as equivalent or claiming access to unavailable ISO clauses?

### Subquestions

- **RQ1.1 — Purpose and object:** What problem, organizational/system object, and intended users does each framework or standard describe?
- **RQ1.2 — Structure:** How does each source organize its content, and what is the appropriate native unit of analysis?
- **RQ1.3 — Governance and responsibility:** What publicly examinable material addresses organizational roles, responsibilities, leadership, oversight, and decision authority?
- **RQ1.4 — Risk and lifecycle:** How are risk identification, assessment, treatment, monitoring, change, and continual improvement represented?
- **RQ1.5 — Evidence and documentation:** What can be established about documented information, records, measurement, evaluation, and traceability from the examined materials?
- **RQ1.6 — Limits:** Which comparisons are defensible, which are non-equivalent, and which remain unknown because source access is incomplete?

## 3. Scope

### 3.1 NIST

Primary subject: **NIST AI Risk Management Framework (AI RMF 1.0), NIST AI 100-1 (2023).**

Primary unit of analysis:
- Functions;
- Categories;
- Subcategories;
- explanatory text needed to interpret those units.

The four Functions—GOVERN, MAP, MEASURE, and MANAGE—must be treated as the framework's own organizing structure. Categories and Subcategories must be recorded under their native parent units.

Initial scope is the AI RMF 1.0 Core and the official framework publication. The Playbook, profiles, crosswalks, implementation resources, and later NIST publications are not silently included. Any decision to add them requires a separately recorded scope extension.

### 3.2 ISO/IEC

Primary subject: **ISO/IEC 42001:2023, Information technology — Artificial intelligence — Management system.**

Permitted sources:
- official ISO and IEC publication/product records;
- official publicly accessible preview material;
- official public descriptions of scope and purpose;
- credible secondary sources, clearly labelled as secondary and not treated as substitutes for the standard.

The complete final-edition normative text is not assumed to be available. No clause-level coverage rating or clause-by-clause completeness claim may be made unless sufficient authorized access to the exact final edition is later established and approved for the intended use.

An FDIS-era crosswalk may be used only as a lead-finding or contextual secondary source. It is not evidence of exact final-edition clause content and is not a normative ISO mapping.

## 4. Prior-work treatment

The following prior work is not repeated:
- historical C1–C20 mapping of NIST AI RMF 1.0 Core;
- public BAES text mapping against the same recovered criteria;
- S01 Axis B evidence-sufficiency coding;
- Axis C residual ambiguity register;
- previous calibration and comparative scope reviews.

These are cited as prior project records, with their original limitations. The recovered historical C1–C20 criteria are not used as the sampling frame or primary analytical instrument for Q1.

The [Prior-Work Gap and Overlap Matrix](00-Prior-Work-Gap-Overlap-Matrix.md) is the controlling scoping record unless superseded by an explicitly approved revision.

## 5. Analytical dimensions

The following dimensions are provisional and must be approved before extraction begins:

1. Stated purpose and intended application.
2. Primary object and level of governance (organization, AI system, lifecycle, process, or other stated unit).
3. Structural organization and normative/functional character of the source.
4. Organizational governance, leadership, roles, and responsibilities.
5. Human oversight and decision-related provisions.
6. AI risk identification, analysis, evaluation, and treatment.
7. Lifecycle processes, monitoring, change, and continual improvement.
8. Documentation, records, measurement, evaluation, and evidence.
9. Implementation, assessment, and assurance mechanisms explicitly supported by the examined source.
10. Source-access and interpretation limits.

Do not assume every dimension exists in both sources or is expressed at the same level. Use “not applicable to this source unit” or “not established from examined material” where appropriate.

## 6. Extraction record

For every extracted statement or structural element, record:

| Field | Description |
|---|---|
| Record ID | Stable sequential identifier |
| Framework | NIST AI RMF 1.0 or ISO/IEC 42001:2023 |
| Source ID | Link to the program source register |
| Source type | Primary official / official supporting / secondary |
| Edition and version | Exact version examined |
| Native location | Function/category/subcategory or publicly visible ISO location |
| Analytical dimension | One or more dimensions from Section 5 |
| Source statement | Concise paraphrase; quote only when necessary and permitted |
| Evidence status | Explicit / indirect / not established / access-limited / not applicable |
| Interpretation | Researcher interpretation, separated from source statement |
| Limitation | Relevant scope or access constraint |
| Verification | Self-checked / independently reviewed / pending |

The extraction record must not convert paraphrase into a purported quotation. Any quotation must be short, accurately attributed, and compliant with source licensing and copyright conditions.

## 7. Analysis procedure

1. Verify the exact edition, identity, and source status of every primary source.
2. Build a source register before substantive extraction.
3. Analyze NIST within its own native structure, beginning with Functions and proceeding through Categories and Subcategories.
4. Analyze ISO only to the depth supported by authorized public material; record unavailable normative content as unknown/access-limited.
5. Complete within-framework summaries before cross-framework comparison.
6. Compare only dimensions that are sufficiently comparable; state differences in purpose, unit, and structure.
7. Record counterevidence, ambiguity, and alternative interpretations.
8. Review all claims against the exact source locations.
9. Produce a limitations-first synthesis.

## 8. Interpretation rules

- A framework's stated purpose is not evidence that every organization implements it.
- A governance outcome is not automatically a task-level authorization requirement.
- Oversight is not automatically equivalent to explicit approval of a particular engineering change.
- Documentation is not automatically sufficient evidence for a claim.
- A management-system requirement and a risk-management framework outcome are not assumed to be equivalent.
- A secondary crosswalk does not override the source's own text.
- Unavailable text is not evidence of absence.
- Conceptual similarity is not proof of equivalence.
- The existence of a topic in a framework does not establish effectiveness.

## 9. Reporting

The report must contain:
- research question and scope;
- source register and exact access boundaries;
- native-structure descriptions;
- within-framework findings;
- dimension-by-dimension comparison where defensible;
- counterevidence and interpretive uncertainty;
- explicit unknowns and access limitations;
- deviations from this protocol;
- bounded conclusion and limitations.

No composite score, weighted total, ranking, conformity claim, or BAES superiority claim will be produced.

## 10. Validation plan

At minimum:
- source and citation verification by the researcher;
- adversarial review of interpretations and non-equivalence claims;
- independent reviewer/second-coder review if feasible and separately arranged.

If no independent reviewer participates, the report must identify the analysis as investigator-side and exploratory. Self-review must not be described as independent validation.

## 11. Stop conditions

Pause Q1 and seek Founder direction if:
- a necessary source is not lawfully accessible;
- a proposed comparison requires reconstructing unavailable ISO clauses;
- the analysis begins to duplicate the historical C1–C20 work;
- a source or method change would materially alter the research question;
- confidential BAES or private project content would be needed;
- an external party requests control over criteria, analysis, findings, or publication.

## 12. Approval gate

This document is a draft. It does not authorize substantive coding, final comparative judgments, external publication, or changes to any other repository.

Q1 may move from **proposed / scoping** to **approved / active** only after the Founder explicitly approves:
1. the research question;
2. analytical dimensions;
3. source boundary;
4. extraction and interpretation rules;
5. validation and reporting plan.

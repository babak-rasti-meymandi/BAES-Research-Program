# Q1 — Prior-Work Gap and Overlap Matrix

**Status:** Preliminary scoping record, prepared from currently inspected public project records.  
**Date:** 2026-11-07  
**Purpose:** Prevent Q1 from repeating or overclaiming the existing NIST/ISO work in the authorization-evaluation project.  
**Important:** This is a program-planning document, not a new framework analysis, rating exercise, or finding about BAES.

## 1. Existing work reviewed

The following public records in [Human-AI-Authorization-Evaluation](https://github.com/babak-rasti-meymandi/Human-AI-Authorization-Evaluation) were inspected for this scoping pass:

- [README](https://github.com/babak-rasti-meymandi/Human-AI-Authorization-Evaluation/blob/main/README.md)
- [02 — Baseline and Comparison Method](https://github.com/babak-rasti-meymandi/Human-AI-Authorization-Evaluation/blob/main/02-Baseline-and-Comparison.md)
- [10 — External Framework Source Register](https://github.com/babak-rasti-meymandi/Human-AI-Authorization-Evaluation/blob/main/10-External-Framework-Source-Register.md)
- [16 — Phase 1 Documentary Reconstruction Audit](https://github.com/babak-rasti-meymandi/Human-AI-Authorization-Evaluation/blob/main/16-Phase-1-Documentary-Reconstruction-Audit.md)
- [22 — Historical C1–C20 Framework Text Coverage](https://github.com/babak-rasti-meymandi/Human-AI-Authorization-Evaluation/blob/main/22-Historical-C1-C20-Framework-Text-Coverage-NIST-ISO.md)
- [24 — Phase 1 Interim Comparative Synthesis](https://github.com/babak-rasti-meymandi/Human-AI-Authorization-Evaluation/blob/main/24-Phase-1-Interim-Comparative-Synthesis.md)
- [25 — Comparative Scope and Criterion-Dependence Review](https://github.com/babak-rasti-meymandi/Human-AI-Authorization-Evaluation/blob/main/25-Phase-1-Comparative-Scope-and-Criterion-Dependence-Review.md)

This is a bounded public-document review, not a full audit of every file or historical revision in that project.

## 2. Gap / overlap matrix

| Research dimension | Prior artifact | What prior work established | Prior method / source boundary | Limitation | Q1 disposition |
|---|---|---|---|---|---|
| Historical C1–C20 criterion set | Recovered criteria; files 22 and 25 | A recovered historical criterion set was used for a criterion-conditioned comparison. | Researcher-supplied hand-over; original date/version and provenance not independently established. | Not normative requirements of BAES, NIST, or ISO; not established as neutral or exhaustive. | **Reuse by citation only.** Do not make it Q1's universal sampling frame or silently revise it. |
| NIST AI RMF 1.0 Core text coverage | File 22, Axis A | Investigator-side mapping of the reviewed Core to historical C1–C20, with criterion-specific rationales and T0–T3/UL rules. | NIST AI RMF 1.0 Core and identified subcategories; bounded to examined text. | Criterion-conditioned; not a full analysis of the whole NIST ecosystem; not independent second-coder verification. | **Do not repeat.** Q1 may add a distinct framework-native structural analysis using Functions, Categories, and Subcategories, linked to prior results. |
| NIST mapping calibration | File 25; later calibration notes in file 22 and project README | Challenge reviews refined ratings and documented why broad concepts do not satisfy narrower event-level criteria. | Investigator-side adversarial review against source text and stated scale. | Still not independent verification; historical narrative sections may preserve superseded intermediate statements. | **Reuse by citation and verify version precedence.** Treat the latest explicit calibration in file 22 and its linked review history as controlling; check stale summaries before quoting ratings. |
| BAES public-text mapping | Files 22 and 25; project README | Public BAES text was mapped to the same recovered historical criteria; T3 was narrowed to C3, C4, C11 and C18 was revised to T2. | Public BAES repository only; no confidential BAES material. | Conceptual text coverage only; no implementation, effectiveness, novelty, or superiority finding. | **Reuse by citation only.** Do not re-score BAES against C1–C20 in Q1. |
| ISO/IEC 42001:2023 source access | Files 10, 22, and 25 | Official public bibliographic/product information and organizational AIMS scope were identified; clause-level C1–C20 coverage remains UL (unreviewed/access-limited). | Official public publication records/preview; FDIS-era crosswalk identified as secondary and not a substitute for final-edition text. | Complete final normative text was not examined; no defensible clause-level positive or negative ratings. | **Carry forward the access limitation.** Do not infer clause coverage, assign T0, or claim full clause-by-clause analysis. Public structural/scope information may be examined with an explicit evidence ceiling. |
| S01 event evidence sufficiency | File 23; file 16; file 24 | Separate Axis B R0–R3 investigator-side assessment of S01-A and S01-B; synthetic evidence contrast; no AI execution provenance established. | Specific synthetic evidence packets; claim-by-claim assessment. | Not a framework-text assessment, real-world incident, human reviewer performance result, or framework effectiveness test. | **Exclude from Q1 rating.** Cite only to explain why framework text and event-level evidence must remain distinct. |
| Residual ambiguity and cross-axis logic | Files 16, 23, 24, and 25 | Axis A text coverage, Axis B packet evidence, and Axis C residual ambiguity were kept separate; no composite score/ranking. | Investigator-side synthesis and alignment checks. | Independent second-coder verification remains outstanding; some synthesis wording may predate later calibration. | **Reuse as methodological caution.** Q1 must define its own dimensions and must not merge unlike constructs. |
| Independent verification | Project README, file 16, and file 25 | Independent second-coder review is identified as a required validation step. | No independent second coder has completed the reported work. | Findings remain investigator-side exploratory judgments. | **Do not claim independent validation.** Decide separately whether Q1 needs an independent reviewer and what resources would be required. |
| Human reviewer study | Project README and phase records | Phase 2 was planned but deferred; no human reviewer assessment has been conducted. | No participant data. | No evidence of reviewer performance, consistency, or benefit from structured review. | **Outside Q1.** Any future human study requires a separate approved protocol in an appropriate existing repository. |

## 3. Candidate gaps remaining for Q1

The prior work does not appear to have completed the following distinct tasks:

1. **NIST native-structure analysis:** a systematic account of the framework's own Functions, Categories, and Subcategories, their relationships, and the levels at which governance, organizational responsibilities, AI-system risk management, and lifecycle activities are addressed. This must not be another C1–C20 crosswalk.
2. **Framework-purpose and unit-of-analysis analysis:** a careful comparison of what NIST AI RMF 1.0 and ISO/IEC 42001:2023 are designed to govern, at what organizational/system level, and what kinds of claims their respective public materials can support.
3. **ISO public-evidence boundary analysis:** a structured account of what official public sources establish about the published standard's identity, purpose, scope, and publicly visible structure—and what remains unknowable without authorized access to the complete final text.
4. **Dimension-specific synthesis:** identify where comparison is defensible, where the frameworks are non-equivalent, and where public sources do not support a conclusion.

These are candidate gaps, not validated research findings. The Q1 protocol must test whether each is meaningful and feasible before analysis begins.

## 4. Proposed incremental Q1 question

> How do the native structures, stated purposes, and publicly examinable materials of NIST AI RMF 1.0 and ISO/IEC 42001:2023 differ in the way they frame organizational AI governance and AI risk management, and what—if anything—can be responsibly inferred about human authority, oversight, evidence, and lifecycle control from those materials without treating the frameworks as equivalent or claiming access to unavailable ISO clauses?

This question is narrower than “Which framework is better?” and broader than the earlier S01 C1–C20 mapping. It does not yet include a new BAES rating.

## 5. Proposed analytical units

| Framework | Primary unit | Permitted secondary material | Do not do |
|---|---|---|---|
| NIST AI RMF 1.0 | Functions → Categories → Subcategories, with the framework's own explanatory text | Official NIST Playbook and other NIST resources only if separately scoped and clearly distinguished from the Core | Do not force ISO clause-level categories onto NIST or present a Core-only analysis as all-NIST coverage. |
| ISO/IEC 42001:2023 | Publicly verifiable document identity, stated scope/purpose, and only those structural elements visible in authorized public sources | Official ISO/IEC/IEC publication pages and carefully identified secondary sources | Do not reconstruct licensed clauses, infer detailed requirements from an FDIS crosswalk, or assign clause-level ratings without sufficient authorized final-edition text. |

## 6. Conditions before Q1 activation

- [ ] Founder approves the incremental research question.
- [ ] Founder approves the source boundary and analytical units.
- [ ] NIST Core and any optional NIST companion resources are explicitly separated.
- [ ] ISO access limitations and permitted-use conditions are recorded.
- [ ] Extraction fields and comparison dimensions are pre-specified.
- [ ] Prior findings are cited as prior work, not silently reused as new results.
- [ ] Reporting language allows positive, negative, mixed, and inconclusive outcomes.

Until these conditions are met, Q1 remains **proposed / scoping**. This matrix does not authorize substantive coding or publication of a comparative conclusion.

## 7. Preliminary scoping conclusion

The most defensible next step is not to repeat the historical C1–C20 mapping. It is to design a framework-native analysis of NIST AI RMF 1.0 and a public-source-limited analysis of ISO/IEC 42001:2023, focused on purpose, structure, level of operation, and the limits of claims concerning authority, oversight, evidence, and lifecycle control.

The earlier S01 project remains a separate scenario-based evaluation. Its findings may inform the questions asked, but must not be used as a shortcut to rate framework effectiveness or BAES added value.

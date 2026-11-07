# Q1 — Preliminary Framework Comparison Memo (Public-Source Bounded)

**Status:** Preliminary; not final synthesis  
**Date:** 2026-11-07  
**Protocol:** Q1 Protocol v1.0  
**Sources:** Q1-NIST-001 to Q1-NIST-003; Q1-ISO-001 to Q1-ISO-002  
**Prior-work boundary:** Does not repeat or recode the historical C1–C20 comparison.

## 1. Purpose of this memo

Record the first defensible comparison that can be made from the examined official public sources. The comparison is intentionally asymmetric: the complete NIST AI RMF 1.0 publication is publicly accessible, while the ISO/IEC 42001:2023 materials examined so far are official publication records and public summaries, not the complete normative text.

This memo is not a final answer to every Q1 subquestion.

## 2. Document type and stated purpose

| Dimension | NIST AI RMF 1.0 | ISO/IEC 42001:2023 | Current comparison status |
|---|---|---|---|
| Document type | NIST describes AI RMF 1.0 as a voluntary AI risk-management framework. | ISO and IEC describe ISO/IEC 42001 as an International Standard specifying requirements and providing guidance for an AI management system (AIMS). | **[EXT]** The sources explicitly identify different document types and stated roles. Do not assume they are interchangeable. |
| Primary organizational context | Organizations designing, developing, deploying, or using AI systems; the framework is intended to be flexible across sectors and use cases. | Any organization, regardless of size, type, or nature, providing or using products or services that utilize AI systems. | **[EXT]** Both address organizations involved with AI, but the available descriptions are not enough to establish identical units of application. |
| Stated purpose | Help manage AI risks and promote trustworthy and responsible AI development and use. | Establish, implement, maintain, and continually improve an organizational AI management system. | **[EXT]** NIST's stated purpose is framed around AI risk management; ISO's public description is framed around an organizational management system. |
| Native structure visible in examined sources | Four Core Functions: GOVERN, MAP, MEASURE, MANAGE; decomposed into 19 Categories and 72 Subcategories. | Official public records confirm the standard identity, edition, purpose, and page count, but do not provide the full final normative structure in the material examined. | **[OBS]** Structural visibility is materially asymmetric. No structural equivalence claim is supportable at this stage. |

## 3. Human authority and oversight

### NIST — explicit source material is available

The NIST AI RMF 1.0 Core includes, among other provisions:
- GOVERN 2.3: executive leadership responsibility for decisions about risks associated with AI-system development and deployment;
- GOVERN 3.2: defining and differentiating human-AI roles and responsibilities, including oversight;
- MAP 2.2: documenting knowledge limits and how outputs may be used and overseen by humans;
- MAP 3.5: defining, assessing, and documenting human-oversight processes in accordance with organizational GOVERN policies;
- Appendix C: differentiating human roles and responsibilities in decision-making and oversight, and identifying further research needs concerning humans' empowerment and incentives to challenge AI outputs.

These are organizational AI-risk governance and oversight provisions in the framework's own terms.

### ISO/IEC 42001 — not yet assessable at clause level

The official public descriptions characterize ISO/IEC 42001 as an organizational AIMS standard and describe its broad purpose. The examined public materials do not provide sufficient final normative clause text to determine how specific requirements address human authority, task-level approval, oversight, delegation, or engineering-change authorization.

**Status:** [UNK] / access-limited for clause-specific conclusions. This is not a negative finding about ISO/IEC 42001.

## 4. Evidence, documentation, and lifecycle

### NIST

The Core distributes documentation, measurement, feedback, review, monitoring, appeal, override, incident response, and change-management elements across the four Functions. MEASURE includes documented metrics and results; MANAGE includes documented risk treatment and post-deployment mechanisms such as appeal and override, incident response, recovery, and change management.

This is an initial synthesis of visible Core text, not a claim that every evidence or traceability question has been exhausted.

### ISO/IEC 42001

The official ISO and IEC descriptions support the broad statement that the standard concerns establishing, implementing, maintaining, and continually improving an AIMS within an organization. They do not, by themselves, establish the detailed content or evidentiary requirements of individual clauses.

**Status:** Broad purpose is [EXT]; detailed clause-level evidence/documentation findings remain [UNK] / access-limited.

## 5. What this comparison does not establish

The examined material does not establish:
- that NIST AI RMF 1.0 is superior or inferior to ISO/IEC 42001:2023;
- that one framework fully covers the other's subject matter;
- that either framework specifies a complete task-level authorization model for AI-assisted software engineering;
- that either framework mandates explicit human approval for every AI-generated code or design change;
- that the absence of an explicit statement in the examined ISO summaries means the final standard lacks such a provision;
- that implementation of either framework guarantees effective governance or oversight.

## 6. Preliminary findings

1. **[EXT]** NIST AI RMF 1.0 is explicitly structured as a voluntary, outcome-oriented AI risk-management framework whose Core is organized around four Functions, Categories, and Subcategories.
2. **[EXT]** ISO/IEC 42001:2023 is explicitly described by ISO and IEC as a management-system standard specifying requirements and guidance for an organizational AIMS.
3. **[INF — bounded]** The sources indicate different native organizing purposes: AI risk-management outcomes and actions in NIST, versus an organizational management-system specification in ISO. This is a distinction in framing, not a ranking.
4. **[EXT]** NIST AI RMF 1.0 has directly inspectable provisions addressing organizational responsibility, human-AI roles, oversight processes, measurement, documentation, feedback, appeal, and override.
5. **[UNK]** The corresponding clause-level position of ISO/IEC 42001:2023 cannot be responsibly characterized from the public materials examined so far.
6. **[EXT]** NIST's current public AI RMF resource page, checked 2026-11-07, states that AI RMF 1.0 is being updated and a revised version is in progress. Q1's analysis is explicitly limited to the 1.0 edition.

## 7. Next steps

- [ ] Complete a source-location-verified extraction of all NIST Core categories/subcategories against Q1 analytical dimensions.
- [ ] Inspect the ISO Online Browsing Platform sample to determine exactly which structural material is publicly visible and permitted to examine.
- [ ] Record any accessible ISO contents/structural information without inferring unavailable clauses.
- [ ] Decide whether credible secondary material adds legitimate context; register it separately and do not treat it as normative text.
- [ ] Conduct an adversarial review of all NIST interpretations that could be mistaken for task-level authorization requirements.
- [ ] Update this memo only when new source evidence is available; retain this version as a dated intermediate record.

## 8. Sources

- [NIST AI 100-1 — AI RMF 1.0 (PDF)](https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.100-1.pdf), especially pp. 1–2, 20–34, and 40–41.
- [NIST publication record — AI RMF 1.0](https://www.nist.gov/publications/artificial-intelligence-risk-management-framework-ai-rmf-10).
- [NIST AI RMF Core resource page](https://airc.nist.gov/airmf-resources/airmf/5-sec-core/), checked 2026-11-07.
- [ISO official catalogue — ISO/IEC 42001:2023](https://www.iso.org/standard/42001).
- [IEC Webstore — ISO/IEC 42001:2023](https://webstore.iec.ch/en/publication/90574).

All claims remain bounded by the sources and portions recorded in the Q1 Source Register.

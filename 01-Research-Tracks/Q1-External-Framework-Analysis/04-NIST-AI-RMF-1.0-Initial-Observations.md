# Q1 — NIST AI RMF 1.0: Initial Native-Structure Observations

**Status:** Preliminary source observations; not a complete extraction or final analysis  
**Source:** Q1-NIST-001 and Q1-NIST-002  
**Access date:** 2026-11-07  
**Protocol:** Q1 Protocol v1.0

## 1. Document identity and stated purpose

**[EXT]** NIST AI 100-1 is the *Artificial Intelligence Risk Management Framework (AI RMF 1.0)*, published in January 2023. NIST's publication record gives 2023-01-26 as the publication date.

**[EXT]** The framework is described as a resource for organizations designing, developing, deploying, or using AI systems to manage AI risks and promote trustworthy and responsible development and use. NIST describes it as voluntary, rights-preserving, non-sector-specific, and use-case agnostic, with flexibility for organizations of different sizes and sectors.

**[INF — limited]** The stated unit of application is not a single engineering task or one AI model in isolation. The framework addresses organizational risk-management practices around AI systems and their lifecycle, while also discussing system-specific contexts.

## 2. Native structure

**[EXT]** The publication is organized into two broad parts:
- Part 1: foundational information, including risk framing, audience, AI risks and trustworthiness, and framework effectiveness;
- Part 2: the AI RMF Core and Profiles.

**[EXT]** The Core has four functions:
- GOVERN
- MAP
- MEASURE
- MANAGE

Each function is decomposed into Categories and Subcategories. NIST explicitly states that the actions do not constitute a checklist and are not necessarily an ordered set of steps.

**[EXT]** GOVERN is designed as a cross-cutting function that informs and is infused throughout MAP, MEASURE, and MANAGE. Risk management is described as continuous and performed throughout AI-system lifecycle dimensions.

**[EXT]** Organizations may apply the functions according to their needs, resources, and capabilities; the framework allows selective use of categories and subcategories. The process is intended to be iterative.

## 3. Governance, roles, and oversight — directly visible examples

The following examples are recorded as source observations, not as a complete inventory:

| Native location | Source-level content (paraphrased) | Relevant dimension |
|---|---|---|
| GOVERN 2.1 | Roles, responsibilities, and communication lines for mapping, measuring, and managing AI risks are documented and clear across the organization. | Organizational roles / accountability |
| GOVERN 2.3 | Executive leadership takes responsibility for decisions about risks associated with AI-system development and deployment. | Leadership / risk decisions |
| GOVERN 3.2 | Policies and procedures define and differentiate roles and responsibilities for human-AI configurations and AI-system oversight. | Human roles / oversight |
| MAP 2.2 | Information about AI-system knowledge limits and how outputs may be used and overseen by humans is documented to support decisions and subsequent actions. | Context / oversight information |
| MAP 3.5 | Processes for human oversight are defined, assessed, and documented in accordance with organizational policies from GOVERN. | Human oversight |
| Appendix C | Human roles and responsibilities in decision-making and oversight need clear definition and differentiation. | Human-AI interaction |

**[EXT]** Appendix C also states that the degree to which humans are empowered and incentivized to challenge AI-system outputs requires further study, and that data about the frequency and rationale for human overrides may be useful to collect.

## 4. Measurement, documentation, and feedback — directly visible examples

**[EXT]** The MEASURE function describes quantitative, qualitative, or mixed-method approaches to analyze, assess, benchmark, and monitor AI risk and related impacts. It includes testing before deployment and regularly during operation.

**[EXT]** The publication connects measurement with documented metrics, methods, uncertainty, formal reporting, and traceability for management decisions. It also notes that independent review can improve testing effectiveness and mitigate internal bias and conflicts of interest.

**[EXT]** Examples in the MEASURE subcategories include documenting test sets and tools, recording performance or assurance measures, and establishing feedback mechanisms through which end users and impacted communities can report problems and appeal system outcomes.

**[EXT]** MANAGE 4.1 includes post-deployment monitoring plans with mechanisms for user input, appeal and override, decommissioning, incident response, recovery, and change management.

## 5. Profiles — source meaning must remain bounded

**[EXT]** NIST AI RMF 1.0 describes use-case profiles as implementations of the Core's functions, categories, and subcategories for a specific setting or application, based on the framework user's requirements, risk tolerance, and resources. It separately describes temporal profiles (current and target states) and cross-sectoral profiles.

**[INF — limited]** “Profile” is a framework-specific term in NIST AI RMF 1.0. Its presence does not establish equivalence with the use, meaning, or architecture of “Profiles” in any other standard or model. No inference about BAES internal specifications is made here.

## 6. Preliminary interpretation boundaries

The observations above show that NIST AI RMF 1.0 contains explicit material concerning organizational risk governance, leadership responsibility for AI risk decisions, human-AI roles, oversight processes, documentation, review, feedback, appeal, and override.

They do **not**, by themselves, establish that the framework:
- defines a complete task-level authorization model for every AI-assisted engineering action;
- requires explicit human approval before every code or design change;
- specifies how to preserve a human's original engineering intent in every delegated task;
- defines a complete protocol for accepting semantic deviations in software changes;
- proves that organizations implementing the framework achieve effective oversight or accountability.

These are scope distinctions, not negative ratings. Any claim of absence requires a complete and properly scoped examination of the relevant source material.

## 7. Remaining extraction work

- [ ] Complete the native-structure inventory for every Category and Subcategory under all four functions.
- [ ] Record exact source locations for each extracted statement.
- [ ] Distinguish the framework's Core from its Profiles section and companion resources.
- [ ] Complete dimension-specific extraction for risk, lifecycle, documentation, assurance, and human oversight.
- [ ] Adversarially review interpretations that might overstate task-level authorization.
- [ ] Reconcile all new observations against the earlier C1–C20 mapping without repeating or silently recoding it.

## 8. Source locations used

- Document identity, date, and update/version policy: NIST AI 100-1, cover and pp. i–ii.
- Stated purpose and voluntary attributes: NIST AI 100-1, pp. 1–2.
- Core structure and four Functions: NIST AI 100-1, pp. 20–21.
- GOVERN categories and subcategories: NIST AI 100-1, pp. 22–23.
- MAP categories and subcategories: NIST AI 100-1, pp. 25–27.
- MEASURE categories and subcategories: NIST AI 100-1, pp. 28–30.
- MANAGE categories and subcategories; Profiles: NIST AI 100-1, pp. 31–34.
- AI actor roles and human-AI interaction: NIST AI 100-1, pp. 35–41.

Primary source: [NIST AI 100-1 PDF](https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.100-1.pdf). Publication metadata: [NIST publication record](https://www.nist.gov/publications/artificial-intelligence-risk-management-framework-ai-rmf-10).

## 9. Current edition status

**[EXT]** NIST's AI RMF resource page, checked on 2026-11-07, states that AI RMF 1.0 is being updated and a revised version is in progress.

Q1 remains scoped to AI RMF 1.0 as a fixed historical edition. The current revision status must be stated in any final report that could otherwise imply AI RMF 1.0 is NIST's latest position.

Current status source: [NIST AI RMF Core resource page](https://airc.nist.gov/airmf-resources/airmf/5-sec-core/), checked 2026-11-07.

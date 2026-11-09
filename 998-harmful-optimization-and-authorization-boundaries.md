# Authorization Boundaries and Harmful Optimization in Human–AI Systems

**Record status:** Exploratory Research  
**Date:** 10 November 2026  
**Research classification:** Non-confidential research case  
**BAES integration status:** Not established

## 1. Purpose

Examine whether a Human–AI system can execute its assigned objectives correctly while those objectives, optimization criteria, or delegated permissions produce harmful effects on people.

The immediate motivating case concerns AI companion chatbots used by minors, particularly systems that use personal memory, emotional profiling, adaptive responses, and engagement optimization in ways that may foster emotional dependency.

This record is a research starting point. It does not establish a BAES requirement, Foundation principle, validated control, or finding about any particular product.

## 2. Motivating Case

A published commentary raises concerns about AI companion systems that can:

- Remember a child's insecurities and personal disclosures.
- Learn emotional triggers and adapt their responses.
- Provide continuous validation and simulate reciprocal emotional relationships.
- Optimize engagement, retention, and session duration.
- Potentially reinforce emotional dependency as a side effect or product objective.

The central concern is not limited to cybersecurity or unauthorized access. A system may protect data and execute its software requirements as designed, while its intended product behavior remains harmful.

The case therefore raises a broader engineering question: can a system be technically secure and operationally compliant while its objectives, authorization boundaries, or effects are unacceptable?

## 3. Core Research Question

**Can a Human–AI system execute its assigned objectives correctly and remain within its delegated technical permissions, yet still constitute an engineering failure because the objectives or delegated permissions themselves are harmful or illegitimate?**

Related questions:

1. Who is authorized to define the system's behavioral objectives?
2. Does an organization's authority to operate a product imply authority to optimize every measurable user behavior?
3. Does permission to personalize interaction include permission to manipulate emotional vulnerabilities?
4. How should conflicts between commercial metrics and human safety be identified?
5. What evidence is needed to reconstruct how objectives, memory, and interaction patterns contributed to an outcome?
6. Who is responsible for identifying and correcting harmful objectives before deployment and during operation?

## 4. Preliminary Distinctions

### 4.1 Technical Security vs. Human Safety

Technical security and human safety are distinct evaluation dimensions. Passing security assessments does not, by itself, establish that a system's objectives or effects are safe for its users.

### 4.2 Correct Execution vs. Legitimate Objectives

A system may faithfully execute its instructions while the instructions themselves are inappropriate, harmful, or outside legitimate authority.

### 4.3 Personalization vs. Manipulation

Personalization adapts a system's behavior to relevant user preferences or needs. Manipulation uses knowledge of a person's vulnerabilities or behavioral tendencies to steer them toward outcomes that may conflict with their interests or autonomy.

The operational boundary between these concepts requires further definition and evidence; it should not be assumed from the presence of personalization alone.

### 4.4 Authorization vs. Outcome Quality

An authorized action may produce an undesirable outcome. A desirable outcome does not retroactively authorize an action that lacked authorization.

These dimensions should be evaluated independently.

## 5. Preliminary Misuse Taxonomy

The following categories are proposed for investigation, not treated as an exhaustive or validated taxonomy:

- **Misuse by User:** A user employs a system in a way that violates applicable permissions or constraints.
- **Misuse by Operator:** An operator uses delegated capabilities beyond legitimate authority or declared boundaries.
- **Harmful-by-Design:** Product objectives, optimization criteria, or interaction architecture systematically encourage or produce harmful effects, even when the system operates as specified.

The third category is especially relevant to this case. It shifts attention from isolated model outputs to the objectives and permissions established across the engineering and operational lifecycle.

## 6. Potential BAES Conceptual Connections

This case may provide an opportunity to examine the applicability of existing BAES concepts without expanding the frozen Foundation Baseline.

- **Human Intent:** What objective is the system intended to serve, and is that objective transparent and consistent with the interests represented?
- **Human Authority:** Who may define, approve, and revise behavioral objectives and constraints?
- **Delegated Execution:** What capabilities are delegated to the model, and where are the boundaries between personalization, persuasion, and manipulation?
- **Evidence and Traceability:** Can the system's relevant objectives, decisions, memory use, and interaction patterns be reconstructed and evaluated?
- **Human Override:** Can responsible human authorities meaningfully constrain, suspend, or reverse harmful behavior?

Human Authority should not be reduced to the authority of the organization deploying the system. The rights, interests, and agency of affected users—including minors—must be considered in the analysis. The legitimate allocation of authority is itself a research question.

## 7. Illustrative Evaluation Scenario

Consider two hypothetical systems:

**System A:** The model departs from its operator's instructions and produces a harmful interaction.

**System B:** The model follows its operator's instructions precisely. The instructions explicitly optimize recurring engagement using remembered emotional vulnerabilities, and the resulting interaction reinforces user dependency.

A model-level execution assessment might identify a deviation in System A but not in System B.

A broader engineering assessment must also examine the legitimacy of the objectives, the authority under which they were approved, the permissions delegated, and the foreseeable effects on affected people.

This scenario is illustrative. It does not establish that any particular system behaves in either way.

## 8. Preliminary Evaluation Dimensions

| Dimension | Questions to investigate |
|---|---|
| Objective legitimacy | Is the objective appropriate, transparent, and defensible? |
| Authority | Who approved the objective and on what basis? |
| Delegation | What capabilities and behavioral permissions were granted? |
| Execution | Did the system remain within its assigned operational boundaries? |
| Human impact | What effects on user autonomy, welfare, and dependency are evidenced? |
| Evidence | Can the relevant design choices and interactions be reconstructed? |
| Intervention | Can responsible parties detect, constrain, and stop harmful behavior? |
| Accountability | Which human roles own the decisions and corrective actions? |

No scoring method or acceptance threshold is proposed at this stage.

## 9. Research Boundaries and Cautions

- Do not infer psychological harm or dependency solely from engagement metrics.
- Do not treat every personalized or emotionally expressive interaction as manipulation.
- Distinguish observed effects, plausible risks, design intentions, and proven causal relationships.
- Avoid treating legal compliance, security certification, or model-level instruction following as sufficient evidence of overall human safety.
- Do not present this exploratory case as proof that BAES already addresses the problem.
- Do not modify the frozen BAES Foundation Baseline as part of this exploratory work.

## 10. Proposed Research Sequence

1. Define the terms objective legitimacy, harmful optimization, emotional dependency, personalization, and manipulation with operational clarity.
2. Identify the actors and authority relationships across product ownership, development, deployment, operation, and user interaction.
3. Construct a lifecycle scenario covering objective selection, delegation, model execution, monitoring, and intervention.
4. Identify the evidence needed to distinguish intended optimization from unintended harmful effects.
5. Evaluate whether existing BAES concepts expose meaningful gaps or distinctions in the scenario.
6. Compare the resulting analysis with relevant external safety and governance approaches, using verified primary sources.
7. Record findings as established, partially supported, not established, or outside the current scope.

## 11. Current Assessment

The case exposes a potentially important distinction:

**Correct Execution of an Objective ≠ Legitimacy of the Objective**

It also suggests that evaluating misuse only as a user's or operator's violation of permissions may be insufficient. The objectives and permissions designed into a system may themselves require scrutiny.

Whether BAES provides a useful and sufficiently precise analytical contribution here remains untested.

**Next intended action:** Develop the scenario into a structured research case and test whether BAES can distinguish execution compliance from objective legitimacy and harmful system-level effects.

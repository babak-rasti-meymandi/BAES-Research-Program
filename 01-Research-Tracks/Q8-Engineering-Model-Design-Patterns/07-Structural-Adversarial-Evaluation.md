# Q8-C07 — Structural Adversarial Evaluation

**Status:** Exploratory  
**Validation:** Not established

## Research question

Can controlled transformations of an engineering model, instruction, workflow, or evidence record reveal material losses of meaning, authority, responsibility, or traceability?

## Candidate transformation classes

- Renaming.
- Semantic substitution.
- Authority substitution.
- Responsibility diffusion.
- Evidence removal.
- Delegation expansion.
- Approval simulation.

This list is provisional and is not a validated taxonomy or a claim of complete coverage.

## Evaluation design questions

- What is the baseline artifact and its accepted meaning?
- Which single transformation is applied?
- What invariant or property is expected to remain stable?
- What counts as a material deviation?
- What evidence supports detection or non-detection?
- How are false positives, false negatives, and ambiguous cases recorded?
- Can the test be independently reproduced?

## Boundaries

Do not claim guaranteed detection or universal coverage. Do not use transformations that expose confidential or restricted material. Separate a test's ability to detect a change from the authority to approve or remediate it.

## Required evidence

Use controlled examples with known transformations, unmodified controls, negative cases, and documented limitations. Any performance claim requires a pre-specified metric and a defensible test set.

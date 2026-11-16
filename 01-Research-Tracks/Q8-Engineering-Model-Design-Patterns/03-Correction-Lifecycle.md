# Q8-C03 — Correction Lifecycle

**Status:** Exploratory  
**Validation:** Not established

## Research question

Which distinct stages are needed to reason about correction of a deviation in an engineering process or model?

## Candidate stages for examination

1. Deviation detection.
2. Classification and impact assessment.
3. Evidence collection.
4. Human review.
5. Authorization decision.
6. Corrective action.
7. Verification of the action and its effects.
8. Closure, reopening, or escalation.
9. Preservation of traceability.

This sequence is a candidate analytical model. The ordering, optionality, and required gates must be tested in context.

## Non-equivalences to preserve

- Detection is not authorization.
- Classification is not approval.
- A correction proposal is not permission to execute.
- Approval of a change is not proof that it was correctly implemented.
- Implementation is not verification.
- Closure is not evidence that no residual risk remains.

## Evaluation questions

- Which transitions require an explicit decision?
- Who or what may propose, authorize, execute, and verify an action?
- How are emergency paths, reversals, and failed corrections handled?
- What evidence is required to establish each transition?
- How are reopened cases and residual uncertainty recorded?

## Boundaries

Do not assume that every domain uses the same lifecycle or that every corrective action requires the same authorization path. No lifecycle model created here grants execution authority.

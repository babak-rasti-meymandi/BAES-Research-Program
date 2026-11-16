# Q8-C08 — Feedback and Decision-State Transitions

**Status:** Exploratory  
**Validation:** Not established

## Research question

How should an engineering model distinguish receipt of new information from an authorized change in the status of a decision?

## Candidate distinctions

- Information received.
- Feedback recorded.
- Evidence assessed.
- Relevance and impact determined.
- Decision reconsideration requested.
- Decision reviewed by an authorized party.
- Change approved or rejected.
- Decision state updated and traceability preserved.

These are candidate distinctions; no universal state machine is asserted.

## Evaluation questions

1. Can new information be recorded without silently changing a decision?
2. What conditions trigger reconsideration?
3. Who is authorized to approve a state transition?
4. How are rejected, superseded, withdrawn, or reopened decisions represented?
5. Can the history of evidence and decisions be reconstructed?

## Boundaries

Feedback alone does not establish approval, authorization, or a state transition. A system's internal status label is not proof that the relevant human or organizational decision occurred.

## Required evidence

Test delayed, contradictory, irrelevant, incomplete, and high-impact feedback. Record how the model handles missing authority, disputed evidence, and failed transitions.

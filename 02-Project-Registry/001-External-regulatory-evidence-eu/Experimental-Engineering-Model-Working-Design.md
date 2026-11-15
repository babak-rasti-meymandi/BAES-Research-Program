# Experimental Engineering Model — Working Design

**Document status:** Working Design — experimental, provisional, and not validated  
**Research project:** BAES-EXT-EVIDENCE-001 — External Regulatory Evidence: AI Governance and Engineering Requirements  
**Relationship to project:** Supporting model-design workstream; not yet adopted as the project's validated assessment method  
**Version:** 0.1 working record  
**Date:** 2026-11-15  
**Classification:** Public research-program working document  
**BAES status:** Not an official BAES model, policy, requirement, or approved extension

---

## 1. Purpose and status

This document records the current design of an experimental engineering assessment model for examining whether a defined AI-assisted engineering activity was performed under identifiable authority, within an established scope, with sufficient execution evidence and appropriate human control.

The model supports evidence-based assessment. It is not a legal decision engine, legal opinion, regulatory compliance assessment, conformity assessment, certification method, or substitute for an authorized human or organizational decision-maker.

The model remains a **Working Design**. Its concepts, rules, tests, state definitions, and proposed architecture have not yet been independently validated. Inclusion in this public research repository does not make the model an official BAES component, establish BAES integration, or imply endorsement by a regulator, public institution, or external organization.

The model must preserve incomplete, negative, mixed, and inconclusive findings. It must not manufacture missing authority, scope, criteria, evidence relationships, or certainty.

### 1.1 Design objective

The central assessment question is:

> How can we establish whether an AI-assisted engineering activity was performed under validly evidenced authority, within its authorized scope, with sufficient execution evidence and appropriate human control?

“Validly evidenced authority” means authority that can be identified and assessed against an applicable governance or authorization basis. The model does not determine legal validity or legal responsibility.

### 1.2 Unit of assessment

The primary unit is a **Defined Engineering Activity**, bounded sufficiently in operational, temporal, and contextual terms to identify the activity and the evidence relevant to it.

The model does not automatically assess an entire organization, AI system, business process, or lifecycle as one indivisible unit. An activity may contain multiple Activity Instances or Execution Segments where evidence and authorization conditions differ.

---

## 2. Architectural overview

The current design has four independent assessment axes. They are not a maturity ladder and must not be averaged into a single score.

### A. Authority and Authorization

Examines the identifiable basis of authority, authorization, delegation, scope, temporal validity, and whether the assessed activity is covered by that authority.

Potential findings include Authorized, Authorization Unproven, Unauthorized (only where positively established), Within Authorized Scope, Outside Authorized Scope (only where positively established), Scope Unproven, Authority Conflict, and Authority Link Unverified.

### B. Engineering Execution Evidence

Examines whether the activity occurred, what was executed, whether execution can be reconstructed, and whether the available evidence supports claims about the actual operation.

Important distinctions:

- Execution Demonstrated is not Authorization Demonstrated.
- Technical Execution Conformance is not Authorization Conformance.
- A timestamp does not by itself prove that an operation completed.
- Action Requested, Action Initiated, Action Executed, Action Completed, and Action Confirmed are distinct events.

### C. Human Control

Examines the availability and operation of human control mechanisms, including intervention, review, stopping, and override.

Three concepts remain separate:

1. **Human Control Capability:** whether a meaningful control capability exists and is available in the relevant configuration.
2. **Human Control Evidence:** evidence that the capability was available and functioned as claimed.
3. **Human Intervention Event:** whether a human intervention actually occurred.

Absence of an intervention event does not establish absence of control. Human Override is important but is not the whole of Human Control. Control Before Action and Control After Action must not be treated as interchangeable.

### D. Accountability Traceability

Examines whether roles, decisions, actions, reviews, acceptances, and accountability relationships can be traced.

Important distinctions:

- Assigned Accountability is not proof that an action was performed.
- A recorded decision is not proof that the recorded person performed the underlying technical action.
- Awareness is not acceptance, authorization, or approval.
- Engineering Accountability is not Legal Responsibility.
- Accountability Traceability is a network of relationships, not necessarily a linear chain.

### 2.1 Independent-axis preservation

Each axis produces its own findings and limitations. A finding on one axis must not be silently used as a finding on another.

For example, an unknown authority origin may stop authorization conclusions while leaving independent execution evidence, control evidence, and traceability observations assessable.

No composite score or average across the four axes is proposed.

---

## 3. Activity characterization, AI role, and scope

### 3.1 AI operational role

AI role is an activity-characterization dimension, not a fifth assessment axis. The current role vocabulary is:

- Information Generation
- Decision Support / Decision Influence
- Decision Execution / Automated Action

These are not necessarily sequential stages. One system may perform more than one role.

The model distinguishes Intended Role, Authorized Role, and Actual Operational Role. A difference between these roles is a deviation to investigate; it does not by itself prove unauthorized activity.

Human Decision Authority does not imply absence of AI Decision Influence. Automated execution does not by itself establish that the AI system made the final decision.

### 3.2 Scope as a shared assessment concept

Scope is relevant across all four axes; it is not a fifth axis. Candidate scope dimensions include Activity Type, Subject, Operational Boundary, Data Boundary, System Boundary, Decision Boundary, Temporal Boundary, and Context Boundary.

Scope may be unspecified, unproven, changed, or established. The model must not infer scope from software configuration alone.

To establish that execution was outside authorized scope, three conditions are required:

1. Established Scope
2. Established Execution
3. Demonstrated Difference

If authorized scope or actual execution is not established, the model must not declare an out-of-scope breach.

### 3.3 Activity segmentation

A single Activity Instance may contain multiple Execution Segments. Authorization or operational conditions may change between segments.

The model should preserve segment-specific timing and findings rather than applying one authorization state to an entire activity without evidence.

A change in software configuration does not automatically constitute a change in authorization scope. A change in Activity Boundary requires recharacterization, not silent rewriting of historical records.

---

## 4. Authority, delegation, conflicts, and time

### 4.1 Authority chain

Relevant concepts include Authority to Delegate, Delegated Authority, Re-delegation / Subdelegation, Configuration Authority, Execution Authority, and AI Operational Role.

Each asserted delegation link should have an identifiable basis, scope, temporal validity, limitations, and traceable supporting evidence.

A failure to establish one link must not automatically be generalized to every other link or to the entire activity. The model must distinguish an AI system acting as a delegated authority-holder from an AI system acting as an execution instrument. Technical capability is not a source of authority.

### 4.2 Authority and scope are distinct

Authorization to generate a score does not automatically establish authorization to execute an automated action based on that score.

Authorization to perform one activity does not automatically transfer to a dependent activity. A single authorization may cover multiple activities only where its evidenced scope supports that conclusion.

### 4.3 Conflicting authority

Potential conflict types include Authority Conflict, Scope Conflict, Delegation Conflict, Temporal Conflict, and Operational Configuration Conflict.

An apparent conflict is not automatically a demonstrated conflict. Activity, subject, scope, time, applicability, and operational effect must be examined.

The model may identify a conflict and record unresolved precedence. It must not invent an authority hierarchy, invalidate an authorization, or appoint itself as the conflict-resolution authority.

### 4.4 Temporal validity and evidence integrity

Keep these time concepts separate: Event Time, Record Time, Effective Time, Observation Time, Activity Time, Evidence Availability Time, and Assessment Time.

Clock offset and drift may affect temporal conclusions. NTP/PTP synchronization does not by itself prove timestamp correctness. Chronological ordering is not necessarily causal ordering.

Authorization effective time, expiry, amendment, and revocation must be assessed against execution time. A later-discovered document may establish an earlier fact, but its discovery date does not itself create authorization.

---

## 5. Evidence architecture

### 5.1 Evidence properties

The model distinguishes Evidence Availability, Evidence Sufficiency, Evidence Authenticity, Evidence Integrity, and Evidence Reliability. These properties are not interchangeable.

Examples:

- Source Attribution is not Event Verification.
- A hash can support integrity comparison but does not prove the original content was true.
- A digital signature does not by itself prove that the claimed real-world event occurred.
- Append-only storage does not prove that all relevant events were recorded.
- Integrity of Records is not Completeness of Records.
- Evidence Sufficiency is Claim-Dependent.

Absence of evidence is not evidence of absence.

### 5.2 Claim-dependent usability

Evidence is not globally “valid” or “invalid” for every purpose. A document may be usable for establishing an authorization date but insufficient to establish that a human reviewer examined a particular output.

Evidence usability must therefore be assessed against the specific Claim and intended evidential use.

### 5.3 Coverage and relationships

**Evidence Coverage** asks whether the necessary elements of a Claim are supported. It is claim-dependent, not document-count-dependent.

**Relational Sufficiency** asks whether relationships among evidence, events, activities, actors, decisions, and outputs are sufficiently established.

The model may represent evidence as an Evidence Set, Evidence Chain, or Evidence Graph. A graph is a useful working representation, not yet a finalized schema.

Potential relationship types include Authorizes, Delegates, Configures, Initiates, Executes, Produces, Reviews, Accepts, Triggers, Records, and AwareOf.

These relationships are not synonyms. In particular:

- AwareOf is not Accepts.
- Accepts is not Authorizes.
- Records is not Executes.

Relationship status may be Established, Supported, Unverified, Conflicted, Not Applicable, or Not Assessed. An observed association alone does not establish a causal or authorization relationship.

### 5.4 Evidence integrity concerns

A hash mismatch, signature issue, provenance gap, or version discrepancy may restrict reliance on a particular evidence item. It must not automatically invalidate unrelated evidence.

A challenged record should remain in the historical record. Its status and permissible use may change in a later assessment version.

---

## 6. Claim decomposition, criteria, and dependencies

### 6.1 Claim decomposition

A compound Claim should be decomposed into independently assessable propositions without changing the original meaning.

Illustrative compound Claim:

“AI was authorized to rank applicants and automatically archive those below a threshold.”

Possible decomposition:

- C1: An authority basis existed.
- C2: The authority covered ranking.
- C3: The authority covered automated archiving.
- C4: The authority was effective at execution time.
- C5: The system performed ranking.
- C6: The system performed archiving.
- C7: The archive action was triggered by the ranking result.

Ranking and archiving authorization are separate. Ranking execution and archiving execution are separate. The relationship between the ranking result and archive action requires its own evidence.

Semantic precision must be preserved. For example, “archived” must not be silently expanded to mean permanently deleted or removed from the recruitment process.

### 6.2 Claim logic

Compound claims may be conjunctive, disjunctive, or conditional. Their logical structure must come from the Claim, applicable criteria, and traceable basis; the model must not invent AND/OR relationships.

For example:

C = (A AND B) OR (D AND E)

Failure to establish one path does not defeat the Claim if another independently sufficient path is established. Conversely, a hypothetical alternative path cannot be used unless its basis is established.

### 6.3 Criteria provenance

Potential criteria sources include Applicable Governance Basis, Activity Authorization, Engineering Requirements, and Assessment Framework. These sources are not interchangeable.

The model distinguishes Authorization Requirement, Engineering Requirement, and Assessment Requirement.

It may identify missing criteria but must not manufacture them. If a criterion required for a final finding is unavailable or its applicability is unverified, the model may perform bounded descriptive or exploratory analysis but must not issue a definitive criterion-dependent finding.

### 6.4 Evidence dependency

Potential dependency types include Authority Dependency, Scope Dependency, Temporal Dependency, and Evidential Relationship Dependency.

A dependency means one assessment element relies on another. Impact means a change to that element actually affects the dependent result. A dependency requires impact review; it does not prove that the result must change.

Dependency types under consideration:

- Essential Dependency
- Supporting Dependency
- Conditional Dependency
- Exclusionary Dependency

If the dependency type is not established, the model must not assume it is essential.

### 6.5 Dependency closure

**Assessment Dependency Closure** is the set of assessment elements connected to a changed element through established and relevant dependencies, and therefore requiring impact review.

Keep two sets distinct:

- **Dependency Closure:** elements requiring review for possible impact.
- **Confirmed Impact Set:** elements for which an actual effect has been established.

A topic-related relationship alone is not a dependency. Closure completeness is always relative to the known and assessed dependency graph; it does not prove that every real-world relationship has been discovered.

---

## 7. Uncertainty propagation

The model distinguishes Uncertainty, Evidence Insufficiency, and Conflict. They are not equivalent.

Potential uncertainty sources include identity, semantics, authority, scope, time, and relationships.

The governing design principle is:

> Uncertainty must be propagated according to established dependencies, not assumed associations.

Potential impact classifications:

- Direct Impact
- Conditional Impact
- No Established Impact

Uncertainty should propagate only to Claims and assessment elements connected by established dependencies. It must not spread to adjacent Claims merely because they concern the same system, person, document, or event.

Important distinctions:

- Authorization Unproven is not Unauthorized.
- Human Control Not Demonstrated is not Human Control Absent.
- Uncertainty propagation is not permission to create a new inference.
- Uncertainty about system behavior is not the same as uncertainty about evidence of system behavior.

The model's primary focus is epistemic uncertainty. Aleatory uncertainty may be relevant to interpreting technical execution but should not be conflated with missing knowledge.

No generic confidence score or averaging across the four axes is proposed.

---

## 8. Assessment revision, change impact, and stability

### 8.1 Change types

Potential assessment changes include Evidence Addition, Evidence Correction, Evidence Reclassification, Criteria Change, Activity Recharacterization, and Dependency Graph Correction.

A change may require reassessment without changing the result.

Distinguish Assessment Reconsideration from Assessment Result Change.

### 8.2 Versioning

Every completed assessment version should remain historically reconstructable. A later version references, but does not overwrite, the earlier version.

Candidate version fields:

- Assessment ID and Version
- Assessment Time
- Activity Reference
- Evidence Set Reference
- Criteria Reference
- Dependency Graph Reference
- Previous Assessment Reference
- Change Reason
- Findings
- Limitations

A document later found to be false or unreliable should not be silently removed from the historical record. Its status should be corrected and dependent findings reassessed.

Historical Assessment Integrity is distinct from Current Assessment Validity.

### 8.3 Cascading changes

A change to an element may affect a Claim, Finding, Activity Characterization, or Dependency Graph and may then affect downstream elements.

When activity characterization changes, review Activity Definition, Claim Decomposition, Evidence Relationships, Scope Mapping, Dependency Closure, and Assessment Version.

A changed activity definition does not silently rewrite history or automatically invalidate prior execution evidence.

### 8.4 Assessment stability

Results should change only in response to relevant changes with established impact. Re-running an assessment with unchanged relevant inputs, criteria, and dependencies should not produce a different result unless the method is inherently nondeterministic; in that case, variance must be recorded.

Useful stability tests include Dependency Consistency, Unrelated Evidence, Evidence Retraction, Alternative Path, Dependency Version, and Uncertainty Propagation tests.

---

## 9. Stop and Escalation Control Layer

Stop conditions are a cross-cutting control layer, not a fixed linear gate sequence. They may activate at different points and restrict only the Claims, branches, evidence, or assessment operations affected by established dependencies.

### 9.1 Action vocabulary

- **Global Stop:** stop all substantive assessment because the assessment unit itself cannot be identified or validated.
- **Claim Stop:** stop assessment of a particular Claim.
- **Branch Stop:** stop a dependency path.
- **Hold:** pause pending a specified input, evidence, or decision.
- **Escalation:** refer an issue to an appropriately authorized or qualified human authority.
- **Restricted Continuation:** continue independent assessment elements.
- **Reassessment Required:** reassess elements whose basis may have changed.

Assessment Stop is not Operational Stop. The model may report that authorization is unverified; it does not thereby issue an operational stop command to a real system. Operational stop decisions and execution belong to an authorized operational authority.

### 9.2 Formalized Stop Rules — working specifications

Each Rule is provisional. Its trigger, scope, action, prohibited inference, resolution condition, and audit record must be tested before validation.

#### STOP-01 — Activity Identity Unresolvable

- **Trigger:** Activity identity or boundary is so unclear that evidence and events cannot be attributed to the assessment unit.
- **Scope:** Global substantive assessment.
- **Action:** Global Stop.
- **Prohibited inference:** Do not construct activity identity from system name or attribute all system logs to the target activity.
- **Resolution:** Establish an identifiable activity boundary or define a narrower independently identifiable assessment unit.
- **Audit record:** Activity reference, ambiguity/conflict, examined evidence, unattributable elements, and stop reason.
- **Boundary:** An unknown local Segment does not automatically require global stop if the remaining activity is identifiable.

#### STOP-02 — Essential Input Unavailable

- **Trigger:** An input required for a particular Claim is unavailable or unusable, with no established sufficient alternative.
- **Scope:** Dependent Claim or branch only.
- **Action:** Hold when a defined input is expected; otherwise Claim/Branch Stop.
- **Prohibited inference:** Do not replace missing input with an assumed value or generalize its absence to independent Claims.
- **Resolution:** Obtain the input or establish a valid alternative path.
- **Audit record:** Input ID, requiredness, dependent Claims, alternatives examined, and reason continuation is blocked.
- **Boundary:** Missing optional input does not by itself trigger a Stop.

#### STOP-03 — Authority Origin Unidentified

- **Trigger:** No authority origin can be identified and examined for the relevant authority Claim.
- **Scope:** Authority-origin Claims and dependent Claims.
- **Action:** Authority Branch Stop.
- **Prohibited inference:** Do not infer authority from job title, successful execution, managerial awareness, lack of objection, or AI capability.
- **Resolution:** Identify an authority origin and obtain sufficient evidence to examine its relationship to the activity.
- **Audit record:** Authority Claim, sources examined, possible origins and their status, missing information, and affected Claims.
- **Boundary:** Does not by itself stop independent execution, human-control, or accountability-traceability assessment. Authority Origin Unidentified is not Unauthorized.

#### STOP-04 — Required Dependency Unestablished

- **Trigger:** A necessary dependency for a Claim is unestablished, unusable, or its relationship to the Claim cannot be established.
- **Scope:** Dependent Claim or branch.
- **Action:** Claim/Branch Stop; examine valid alternative paths where the Claim logic supports them.
- **Prohibited inference:** Do not assume all dependencies are conjunctive or treat every related item as essential.
- **Resolution:** Establish the required dependency, establish a sufficient alternative path, or establish that the dependency is not necessary.
- **Audit record:** Claim ID, dependency ID/type, logic, prerequisite status, alternatives, and reason for action.

#### STOP-05 — Material Conflict Unresolved

- **Trigger:** Relevant sources or claims are materially inconsistent and cannot be accepted together without affecting the assessment.
- **Scope:** Conflicted Claims and branches.
- **Action:** Hold and, where resolution requires authority, Escalation; independent Claims may continue.
- **Prohibited inference:** Do not automatically prefer the newest, most formal-looking, or highest-ranking source without an established precedence basis.
- **Resolution:** Resolve the conflict, establish applicability differences, or record a competent authority's decision and its basis.
- **Audit record:** Conflicting sources, conflict type, scope/time/applicability, affected Claims, precedence basis, and resolution status.
- **Boundary:** Apparent Conflict must be distinguished from Demonstrated Conflict.

#### STOP-06 — Criteria Basis Unavailable

- **Trigger:** A criterion necessary for a finding cannot be identified, accessed, versioned, or shown to apply.
- **Scope:** Criterion-dependent findings only.
- **Action:** Stop the dependent final finding; bounded descriptive or exploratory analysis may continue.
- **Prohibited inference:** Do not manufacture criteria, substitute a generic convention for a required criterion, apply a later criterion retrospectively without basis, or convert missing criteria into proof of violation.
- **Resolution:** Identify the criterion, establish applicability, and determine the relevant version/effective time.
- **Audit record:** Claim, criterion/source/version, applicability issue, effective time, affected findings, and permitted limited analysis.

#### STOP-07 — Evidence Integrity Concern

- **Trigger:** A specific, relevant concern undermines reliance on an evidence item for a Claim.
- **Scope:** Challenged evidence and Claims dependent on it.
- **Action:** Restrict or hold reliance on the evidence; stop only Claims lacking a sufficient independent path.
- **Prohibited inference:** Do not infer truth from a hash, event occurrence from a signature, completeness from append-only storage, or invalidity of all evidence from one challenged item.
- **Resolution:** Resolve the integrity/authenticity concern, find a reliable replacement, or establish an independent sufficient path.
- **Audit record:** Evidence ID/version/source, concern type, examinations, status, affected Claims, and alternatives.
- **Boundary:** A hash mismatch may arise from format conversion or version mismatch; it is not automatically proof of tampering.

#### STOP-08 — Scope Cannot Be Established

- **Trigger:** The authorized scope or relevant version at execution time cannot be established.
- **Scope:** Claims about within-scope/out-of-scope execution.
- **Action:** Stop conclusions about scope conformance; independent execution Claims may continue.
- **Prohibited inference:** Do not declare Outside Authorized Scope without established scope, established execution, and demonstrated difference.
- **Resolution:** Establish the applicable scope/version/time and compare it with established execution.
- **Audit record:** Scope Claim, versions, effective times, Activity Instance, limitations, and permitted conclusion.

#### STOP-09 — Activity Boundary Changed

- **Trigger:** New evidence calls the prior Activity, Activity Instance, Segment, or operational boundary characterization into question.
- **Scope:** Activity characterization and dependent Claims.
- **Action:** Recharacterization Required; recalculate Dependency Closure and selectively reassess.
- **Prohibited inference:** Do not silently rewrite historical activity definitions, assume a software change creates a new activity, or invalidate prior evidence automatically.
- **Resolution:** Establish the revised boundary and relationships, update Claim decomposition/dependencies, and create a controlled assessment version.
- **Audit record:** Prior definition, new evidence, revised characterization, affected Claims, graph changes, and historical references.

#### STOP-10 — Assessment Reconstruction Incomplete

- **Trigger:** Necessary historical inputs, criteria, method, versions, relationships, or change records are missing such that full reconstruction cannot be supported.
- **Scope:** Claims about historical reconstruction and reproducibility.
- **Action:** Restrict the reconstruction claim; do not claim full reproducibility. Independent findings are not automatically invalidated.
- **Prohibited inference:** Do not reconstruct missing inputs from the final output or infer that a non-reproducible finding was necessarily wrong.
- **Resolution:** Recover historical records or explicitly limit the reconstruction claim to what is supported.
- **Audit record:** Assessment ID/version, recovered and missing elements, impact, reconstruction level, and limitations.

#### STOP-11 — Unresolved Dependency Structure

- **Trigger:** The model cannot establish which dependencies are essential, supporting, conditional, or alternative, or cannot establish the relevant AND/OR logic.
- **Scope:** Claims relying on the unresolved dependency structure.
- **Action:** Claim/Branch Stop or restricted continuation.
- **Prohibited inference:** Do not invent AND/OR logic or treat every graph cycle as circular justification.
- **Resolution:** Establish the dependency logic from the Claim, criteria, and traceable basis.
- **Audit record:** Disputed dependency structure, alternatives, affected Claims, and reason it remains unresolved.
- **Distinction:** STOP-11 concerns uncertainty about the dependency structure; STOP-04 concerns an unestablished prerequisite within a known dependency structure.

#### STOP-12 — Assessment Control Authority Unverified

- **Trigger:** A person or mechanism requests a controlled assessment action—such as lifting a governance restriction, accepting a finding, or changing an assessment result—but its authority for that specific action is unverified.
- **Scope:** The requested controlled change.
- **Action:** Hold the requested change and escalate where necessary.
- **Prohibited inference:** Do not infer authority from job title, technical access, or the fact that someone commissioned the assessment.
- **Resolution:** Establish the relevant authority or have the action performed by a competent authorized person.
- **Audit record:** Request, requester identity/role, requested action, authority basis, and decision.
- **Boundary:** Routine correction of an evaluator's own draft calculation need not require organizational approval; required authority depends on the nature of the action.

### 9.3 Rule interaction and precedence

Multiple Rules may be active simultaneously. Rule activation, interaction, precedence, and resolution are separate concepts.

Potential interaction types: Independent, Overlapping, Dependency-Linked, Sequential, and Mutually Constraining.

Potential interaction statuses: Rule Interaction Compatible, Rule Interaction Overlapping, Rule Interaction Unresolved, and Rule Interaction Conflicted.

The presence of multiple active Rules is not itself a conflict.

**RULE-INT-01 — Dependency-Based Rule Precedence (Draft):**

When multiple Stop Rules are active, the order of review and action should be determined by established prerequisites, impact scope, and valid dependencies—not merely by Rule number or apparent severity.

Constraints:

1. Operational precedence does not erase another Rule's finding.
2. Resolving one Rule does not automatically resolve independent Rules.
3. Effects remain bounded by established dependency closure.
4. If precedence cannot be established, record Rule Precedence Unestablished; do not guess.
5. No Rule creates authority by virtue of precedence.

### 9.4 Dependency-Bounded Continuation

The model may continue an assessment step only when the necessary preconditions for that step are established. A missing or conflicted prerequisite restricts only dependent Claims and branches unless the identity or assessability of the entire activity is compromised.

The model must not invent missing prerequisites, turn missing evidence into proof of breach, or extend a branch stop to independent results.

---

## 10. Stop Rule test matrix

Stop Rules require positive, negative, and boundary testing.

### 10.1 Test dimensions

| Test dimension | Question |
|---|---|
| Trigger Accuracy | Was the Rule activated only when its trigger was met? |
| Scope Accuracy | Were only dependent Claims/branches affected? |
| Action Accuracy | Was the correct Stop, Hold, Escalation, or restricted continuation selected? |
| Inference Safety | Were prohibited inferences avoided? |
| Resolution Accuracy | Did resolution affect only elements whose dependencies justified reassessment? |

### 10.2 Minimum positive/negative/boundary cases

| Rule | Positive test | Negative test | Boundary test |
|---|---|---|---|
| STOP-01 | Activity cannot be identified or evidence attributed | Activity is identified but one Segment is unknown | Narrower identifiable unit can be assessed |
| STOP-02 | Claim-essential execution time is unavailable | Optional descriptive input is missing | Valid sufficient alternative input exists |
| STOP-03 | No authority origin is identifiable | Origin known but delegation record is missing | Origin known, temporal validity unproven |
| STOP-04 | Necessary prerequisite is unestablished | Missing item is only supporting | One valid OR path remains established |
| STOP-05 | Applicable sources materially conflict | Sources concern different scopes | One source is outside the relevant period |
| STOP-06 | Required criterion is unavailable | Descriptive analysis needs no criterion | Later criterion is not automatically retrospective |
| STOP-07 | Sole supporting record has an unresolved integrity mismatch | Hash alone does not establish original truth | Independent evidence path remains available |
| STOP-08 | Applicable scope cannot be established | Scope and execution are established and consistent | Execution differs but authorized scope is unknown |
| STOP-09 | New evidence changes activity boundary | Software version changes without boundary change | New Segment is identified but its relationship is unresolved |
| STOP-10 | Historical inputs/method cannot be reconstructed | Missing parameter is demonstrably irrelevant | Partial reconstruction remains possible |
| STOP-11 | AND/OR dependency logic is unknown | Dependency logic is explicit | A cycle exists but is not necessarily circular justification |
| STOP-12 | Unverified person requests controlled governance change | Authorized evaluator corrects own draft calculation | Requester has authority for one action but not another |

### 10.3 Temporal testing

Tests should distinguish T0 (state before change), T1 (time new evidence or information is received), and T2 (state after controlled reassessment).

A test must verify not only the final label but also whether the model reassessed the correct dependent elements and preserved historical states.

### 10.4 Test outcome versus assessment finding

Keep these separate:

- **Test Result:** whether the model behaved according to the Rule.
- **Assessment Finding:** what the model establishes about the assessed activity.

A successful test does not validate the factual truth of a scenario's claims.

---

## 11. Assessment State Machine

### 11.1 Multi-level state architecture

A single status for the entire assessment is insufficient. The model uses separate state dimensions at different levels:

1. Assessment State
2. Claim Assessment State
3. Dependency / Branch State
4. Evidence State
5. Stop Rule State

These levels must not be collapsed into one status field.

### 11.2 Assessment-level states

Proposed states:

- **Draft:** assessment defined but not ready.
- **Ready:** initiation prerequisites are met.
- **In Progress:** substantive assessment is underway.
- **Partially Completed:** some elements have reached an assessment outcome while others remain open.
- **On Hold:** one or more parts are temporarily paused.
- **Stopped:** substantive assessment is stopped within the relevant scope.
- **Completed:** assessment is complete within its defined scope.
- **Cancelled:** assessment was cancelled through a recorded authorized action.
- **Superseded:** a later assessment version has replaced this version as the current assessment record.

Stopped is not necessarily terminal. A later controlled reassessment may be initiated. Reporting, history preservation, and recording limitations may continue even when substantive assessment is stopped.

### 11.3 Claim-level states

Proposed states:

- Not Started
- Ready
- In Progress
- Finding Established
- Finding Partially Established
- Finding Not Established
- Unproven
- On Hold
- Stopped
- Not Applicable
- Superseded

Distinctions:

- **Unproven:** available evidence is insufficient to establish or reject the Claim.
- **Finding Not Established:** after applying the available relevant criteria and evidence, the Claim was not established.
- Neither state automatically proves the opposite Claim.
- A compound Claim may be Partially Established while its decomposed Claims retain independent states.

### 11.4 Dependency / Branch states

Proposed states:

- Not Evaluated
- Available
- In Progress
- Established
- Not Established
- Blocked
- On Hold
- Invalidated
- Superseded

Blocked is not the same as Not Established. A blocked path has not necessarily failed. Invalidated means the prior basis for a path is no longer valid; it does not automatically invalidate every Claim that previously referenced it.

### 11.5 Evidence states

Proposed states:

- Received
- Identified
- Under Review
- Usable
- Restricted
- Challenged
- Rejected for Specific Claim
- Superseded

Evidence usability is Claim- and purpose-dependent. A record may be usable for one Claim and restricted for another.

### 11.6 Stop Rule states

Proposed states:

- Inactive
- Triggered
- Active
- Resolution Pending
- Resolved
- Reopened
- Superseded

Triggered and Active may be distinct where a potential condition is detected but its applicability or materiality still requires examination. A Rule may specify precautionary action during that examination.

### 11.7 State dimensions must remain separate

| Dimension | Examples |
|---|---|
| Process Status | Draft, Ready, In Progress, Completed, Cancelled |
| Execution Control Status | Active, On Hold, Stopped, Restricted |
| Finding Status | Established, Not Established, Unproven, Partially Established |
| Version Status | Current, Superseded |
| Dependency Status | Available, Blocked, Established, Invalidated |
| Rule Status | Inactive, Active, Resolution Pending, Resolved, Reopened |

A Claim can be process-complete while its finding remains Unproven and its control status remains Restricted. This is not inherently contradictory.

### 11.8 Completion semantics

Completed means the assessment process has ended within its defined scope. It does not mean every Claim is established or every uncertainty resolved.

Proposed completion classifications:

- **Completed — Fully Assessed:** every Claim in scope has been assessed.
- **Completed — With Unresolved Findings:** assessment is complete but unresolved matters remain.
- **Completed — With Restricted Scope:** assessment was completed within a transparently narrowed scope.

These are completion classifications, not additional process states.

Before marking an Assessment Completed:

1. Assessment identity and scope are sufficiently defined.
2. Every in-scope Claim has an explicit status, including unresolved or unproven status.
3. Active Rules and residual limitations are recorded.
4. Dependencies needed for reported findings have been assessed.
5. Required outputs and rationale records are preserved.
6. The accountable evaluator confirms process completion.

A Claim may be final while another Claim is on hold. The overall Assessment state must be derived from the defined scope and the state of its constituent elements, not copied from one Claim.

### 11.9 Continuation, revision, and new assessment

Distinguish:

- **Assessment Continuation:** an unfinished assessment proceeds after an input or temporary blocker is addressed.
- **Assessment Revision / Reassessment:** a completed or recorded assessment is reviewed against new evidence, corrected relationships, changed criteria, or a revised method. The previous version remains preserved.
- **New Assessment:** a materially different objective, activity, or scope requires a separate assessment record.

Reassessment is an operation; Assessment Version is a historical record.

A changed Activity Boundary does not automatically require a new Assessment. First perform controlled recharacterization and determine whether revision or a new assessment is justified.

### 11.10 State transition records

Every state transition should be tied to a recorded event and contain:

- Transition ID
- Source State
- Trigger Event
- Preconditions
- Target State
- Affected Scope
- Evidence Basis
- Rule Reference
- Assessment Version
- Transition Record

Receiving a document does not itself establish an authorization Claim. For example, a Claim on hold because authority origin is unknown may move to In Progress when a source is identified; it must not jump directly to Finding Established without examining validity, scope, delegation, and time.

### 11.11 State consistency invariants

| ID | Invariant | Requirement |
|---|---|---|
| ST-INV-01 | Historical State Preservation | Historical states are retained, not overwritten. |
| ST-INV-02 | Independent Claim State | Each Claim retains its independent state. |
| ST-INV-03 | Dependency-Bounded Transition | State changes propagate only through established dependencies. |
| ST-INV-04 | No Implicit Resolution | Resolving one Rule does not resolve independent Rules. |
| ST-INV-05 | Completion Integrity | Completed does not imply all findings are resolved. |
| ST-INV-06 | Version Integrity | A superseding version does not delete the prior version. |
| ST-INV-07 | Evidence-State Specificity | Evidence usability is Claim- and purpose-dependent. |
| ST-INV-08 | No Unauthorized Transition | Controlled changes require the relevant authority. |
| ST-INV-09 | State-Transition Traceability | Every state change has a recorded event and basis. |
| ST-INV-10 | No False Finality | Stop, completion, and non-establishment are not conflated. |

---

## 12. Model inputs and outputs — current working specification

### 12.1 Requiredness is assessment-dependent

Input requiredness is not identical for every activity or Claim.

- **Core Required Inputs:** needed to initiate a meaningful assessment.
- **Conditional Required Inputs:** required for particular Claims or assessment types.
- **Optional Inputs:** useful but not necessary for the defined assessment.
- **Unavailable / Not Provided:** availability status, not an input requiredness class.

### 12.2 Input groups

**A. Activity Identification**

- Activity Reference — Required
- Activity Description — Required
- Activity Objective — Required
- Activity Boundary — Required
- Activity Time Range — Conditional
- Activity Instance Reference — Conditional
- Activity Segments — Conditional

**B. Human and Organizational Context**

- Human Actor Identity — Conditional
- Actor Role — Conditional
- Organizational Context — Conditional
- Authority Source Reference — Conditional
- Delegation Records — Conditional
- Approval Records — Conditional

**C. AI System**

- AI System Identity — Conditional
- AI Operational Role — Conditional
- Model Identifier and Version — Conditional
- Software Version — Conditional
- Configuration — Conditional
- Model Parameters — Conditional
- Tool / External Service References — Conditional

Version information becomes required when a Claim concerns version-specific behavior, multiple versions in one execution, changed behavior, conformance to an authorized version, or exact historical reconstruction. Missing version information should restrict dependent Claims, not automatically stop the entire assessment.

**D. Authority and Scope**

- Governance Basis — Conditional
- Authorization Record — Conditional
- Delegation Chain — Conditional
- Authorized Scope — Conditional
- Scope Version — Conditional
- Effective Time — Conditional
- Expiry / Revocation — Conditional

**E. Execution and Evidence**

- Execution Records — Conditional
- System Logs — Conditional
- Input / Output Records — Conditional
- Event Timestamps — Conditional
- Evidence Source — Required for each supplied evidence item
- Evidence Identity — Required for each supplied evidence item
- Evidence Version — Conditional
- Evidence Integrity Data — Conditional
- Evidence Relationships — Conditional

**F. Assessment Control**

- Assessment Objective — Required
- Claims to Assess — Required
- Applicable Criteria — Required for criterion-dependent final findings
- Criteria Version — Conditional
- Assessment Method — Required
- Previous Assessment Reference — Conditional
- Evaluator Identity / Role — Required for accountable assessment

Candidate input record fields: Input ID, Input Type, Value or Reference, Source, Version, Availability Status, Applicability, Requiredness, Integrity Status, Related Claims, and Limitations.

### 12.3 Model outputs

Proposed assessment outputs:

1. Assessment Identification
2. Input Validation Report
3. Four-Axis Findings
4. Stop and Escalation Report
5. Reproducible Assessment Rationale Trail
6. Assessment Synthesis
7. Assessment Change History

The principal output unit is a **Claim Assessment Record**, containing Claim ID and original/decomposed Claim; Claim Semantic Integrity status; applicable criteria and provenance; evidence references, versions, sources, and relevant locations; evidence relationships and their status/basis; assessment operations and applied rules; finding and supporting/contradicting evidence; unresolved issues and limitations; evaluator/reviewer and acceptance status; human intervention and revision references.

The term **Reproducible Assessment Rationale Trail** does not mean private chain-of-thought disclosure. It means a reviewable record of claims, evidence citations, relationships, applied criteria, observable assessment operations, concise rationale, decisions, and limitations.

---

## 13. Illustrative integrated scenario — EU-S-01

The following is a fictional design-test scenario, not a real audit or factual finding.

A fictional HR system receives CVs, ranks applicants, and automatically archives some applicants below a threshold. The scenario is used to test the model's ability to separate authorization, execution, human control, and accountability.

Illustrative elements:

- A1: CV intake and processing
- A2: ranking
- A3: automated archiving below a threshold
- A4: review/recovery capability
- M1: hiring manager
- S1: AI system
- P1: organizational policy
- L1: logs
- D1: delegation document

Test observations include:

- The authority origin is initially unidentified.
- Ranking and archive logs are available.
- System version is later identified, but exact operational configuration is not.
- A document describes an override capability, but its link to the executed configuration is not established.
- A manager is aware of the operation, but formal acceptance or authorization is not established.
- A policy appears to restrict archiving without human review, but applicability, precedence, meaning of “archived,” and temporal validity require examination.
- New evidence suggests ranking and archiving may be separate services or activities.
- A previously inferred Accepts relationship is corrected to AwareOf.

Expected assessment behavior:

- Authority conclusions remain unproven until their basis is established.
- Execution evidence may be assessed independently.
- Human Control is not demonstrated merely by a document describing a capability.
- Awareness does not establish acceptance or authorization.
- “Archived” is not silently interpreted as permanent deletion.
- Activity recharacterization triggers dependency review but does not automatically invalidate execution records.
- Correcting an evidence relationship affects dependent Claims, not independent findings.

Illustrative four-axis synthesis:

- A — Authority and Authorization: Authorization Unproven / Conflict Unresolved where applicable.
- B — Engineering Execution Evidence: Execution Demonstrated, subject to Claim-specific scope and evidence limitations.
- C — Human Control: Human Control Not Demonstrated.
- D — Accountability Traceability: Traceability Incomplete.

These are illustrative outcomes for testing model behavior, not validated findings about a real organization or system.

---

## 14. Cross-cutting design invariants

The current working set includes:

- **INV-01 Authority Non-Inference:** authority is not inferred from role, capability, awareness, successful execution, or silence.
- **INV-02 Independent Axis Preservation:** findings on one axis do not automatically determine another.
- **INV-03 Dependency-Bounded Propagation:** uncertainty and change propagate only through established dependencies.
- **INV-04 Historical Assessment Preservation:** prior assessment states and versions remain recoverable.
- **INV-05 Claim Semantic Integrity:** decomposition and reassessment do not silently change the original Claim's meaning.
- **INV-06 Evidence Relationship Precision:** awareness, review, acceptance, authorization, execution, and recording remain distinct.
- **INV-07 No False Completion:** completion does not imply every Claim is established or every issue resolved.
- **INV-08 No Manufactured Criteria:** missing criteria are identified, not invented.
- **INV-09 No False Scope Breach:** out-of-scope findings require established scope, execution, and demonstrated difference.
- **INV-10 No Implicit Rule Resolution:** resolving one restriction does not resolve unrelated restrictions.

These invariants remain proposed and require positive, negative, boundary, and interaction testing.

---

## 15. Open design work and validation sequence

The following work remains open. Inclusion here is not a claim of completion or validation.

1. **Assessment Event Model:** define Event versus State, event identity, duplicate/conflicting events, event ordering, effective time, record time, and event-to-state transitions.
2. **Event-driven reconstruction:** test whether historical assessment states can be reconstructed from retained events, evidence versions, criteria, and dependency graph versions.
3. **Stop Rule validation:** execute positive, negative, boundary, temporal, and multi-Rule interaction tests for all 12 Rules.
4. **Rule precedence validation:** test dependency-based operational precedence without merging independent findings.
5. **State-machine validation:** test valid/invalid transitions, partial completion, hold/stop coexistence, reassessment, cancellation, and supersession.
6. **Input schema:** convert the current input groups into a structured schema with claim-dependent requiredness and explicit unavailable states.
7. **Output schema:** define machine-readable and human-reviewable assessment records.
8. **Independent reconstruction test:** determine whether another evaluator can reconstruct the assessment from the retained records without access to private model reasoning.
9. **Adversarial testing:** test false linkage, over-propagation, under-propagation, semantic drift, false completion, and unauthorized state changes.
10. **Scope and publication review:** ensure public outputs do not include confidential or restricted BAES material and do not imply legal or regulatory conclusions beyond the evidence.

### 15.1 Proposed validation criteria

A rule, state transition, or assessment capability should not be treated as validated merely because it has been described. At minimum, validation should examine positive trigger behavior, negative trigger behavior, boundary behavior, interaction with other Rules, dependency-scope accuracy, historical preservation, resolution behavior, and reproducibility/independent reconstruction where applicable.

### 15.2 Current maturity statement

The design currently has a coherent provisional architecture for four-axis assessment, claim decomposition, evidence relationships, dependency-bounded uncertainty, Stop Rules, Rule interaction, and multi-level Assessment State.

It has not yet completed the Event Model, schema design, full test execution, independent reconstruction, or validation. No claim of operational readiness or regulatory suitability is made.

---

## 16. Governing caution

The model should prefer an explicit, bounded **not established** result over an unsupported conclusion.

It should identify missing authority, criteria, evidence, relationships, or control without manufacturing them; preserve findings that remain independently supportable; and restrict uncertainty or reassessment to dependencies that are actually established.

The design's central discipline remains:

> Uncertainty must be propagated according to established dependencies, not assumed associations.


---

## 17. Evidence Extraction and Evidence Object Model

**Status:** Working design — provisional and not validated  
**Design scope:** Evidence extraction, provenance, transformation lineage, claim-specific use, lifecycle, and preservation  
**Boundary:** This section does not establish the truth of source content, validate an extraction tool, or define a universal evidence-weighting scheme.

### 17.1 Three distinct objects

The design distinguishes three entities:

1. **Input Object:** the received source artifact or record, such as a PDF, configuration file, log, database record, message, image, or external record.
2. **Extracted Information Object:** a specific content item obtained from an Input Object through extraction, parsing, OCR, transcription, translation, summarization, or another transformation.
3. **Evidence Object:** an identifiable evidential item assessed for a specific claim-related use, with traceable source lineage, content, relationships, and limitations.

These entities must not be collapsed. One Input may yield multiple Extracted Information Objects. One Extracted Information Object may be considered for multiple Claims. One Evidence Object may draw on multiple Inputs or extracted items. One Input may contain information that supports, contradicts, or is irrelevant to different Claims.

An Evidence Object is not necessarily a single sentence. It may represent a value, record, technical output, event record, or bounded composite of information. Its boundary should be determined by its evidential purpose and semantic coherence, not merely by file or text boundaries.

### 17.2 Input Object preservation

An Input Object represents a received source, not the truth of what the source asserts.

Candidate fields:

- Input ID
- Original Source Reference
- Source Identity (asserted and/or established status)
- Submitted By
- Received By
- Received Time
- Source Time, if available
- Original Format
- Content Fingerprint
- Version Reference
- Preservation Status
- Declared Purpose
- Access / Availability Status

Submitted By, Received By, and Source Identity are distinct. The submitter is not presumed to be the source author or originator.

A converted or normalized file must not replace the original Input. Converted artifacts are separately identified and linked to the source Input. Input version changes do not silently replace historical versions.

### 17.3 Extracted Information Object

Extracted Information is a distinct object because extraction and transformation can introduce omissions, errors, ambiguity, or semantic drift.

Candidate fields:

- Extracted Information ID
- Source Input ID
- Source Location (page, paragraph, line, record, field, image region, or time range)
- Extraction Method
- Extracted Content
- Content Type
- Language
- Transformation History
- Extraction Tool / Model / Version
- Parameters and Configuration
- Extraction Time
- Extraction Fidelity Status
- Known Limitations
- Uncertainty Notes

Candidate extraction methods include Direct Text Extraction, OCR, Structured Data Parsing, Manual Transcription, Translation, Summarization, Model-Assisted Extraction, and Data Transformation.

Original Text, OCR Output, Translation, and Summary are not interchangeable. Each transformed output must be separately identified and linked to its immediate input and ultimate source lineage. A summary is not presumed to preserve all information in its source; a translation is not presumed semantically exact; OCR is not presumed error-free.

### 17.4 Extraction is not verification

The design distinguishes:

- **Extracted Information:** content obtained from a source.
- **Evidence Candidate:** information considered potentially relevant to a defined Claim.
- **Assessed Evidence:** information whose provenance, content, applicability, limitations, and intended use have been assessed for a particular Claim.

Extraction alone does not establish source authenticity, event occurrence, semantic correctness, Claim applicability, or evidence sufficiency.

The following are distinct:

- Extraction is not Verification.
- Verification is not Applicability.
- Applicability is not Sufficiency.

A proposition appearing in an Input does not automatically become a verified fact or an established Claim.

### 17.5 Evidence Object

Candidate fields:

- Evidence ID
- Evidence Type
- Evidence Content Reference
- Source Input References
- Extracted Information References
- Extraction Lineage
- Evidence Proposition
- Source Attribution Status
- Content Integrity Status
- Extraction Fidelity Status
- Claim Applicability
- Assessment Status
- Limitations
- Version
- Supersession / Retraction References

**Evidence Proposition** is distinct from the assessed **Claim**. The proposition describes what the evidence item records, indicates, or supports; the Claim is the proposition being assessed. A relationship between them must be established rather than assumed.

For example, a log may record that an Archive operation was executed. That does not by itself establish that the operation belonged to the defined Activity, was triggered by a particular ranking result, or was authorized.

### 17.6 Multi-source lineage

An Evidence Object may be supported by one or multiple Inputs or Extracted Information Objects.

The design distinguishes:

- **Single-source evidence:** one source supports the relevant evidential item.
- **Multi-source evidence:** multiple sources contribute different elements to a composite evidential item.
- **Corroborative evidence:** multiple sources provide support for the same or overlapping propositions.

The contribution and role of each source must remain separately traceable. Combining sources does not establish that they are independent, mutually corroborative, or causally related.

Two reports generated from the same underlying database are not presumed to be independent sources. Source independence must be established from provenance and relevant production dependencies, not inferred from the number of files or records.

### 17.7 Source attribution and transformation lineage

Each extraction or transformation should retain a traceable relationship to its source and source location.

Candidate Transformation Record fields:

- Transformation ID
- Input Object Reference
- Output Object Reference
- Transformation Type
- Tool / Model / Version
- Parameters and Configuration
- Execution Time
- Performed By
- Source Location
- Known Limitations
- Validation Status

Lineage should permit an assessor to trace an Evidence Object through its extracted and transformed representations to the original source. This is provenance reconstruction, not a claim that every transformation is mathematically reversible.

Where a transformation is lossy or exact source reconstruction is unavailable, that limitation must be recorded and considered in the relevant assessment.

### 17.8 Evidence types and claim relationships

Candidate Evidence Types:

- Direct Evidence
- Derived Evidence
- Composite Evidence
- Corroborative Evidence
- Contradictory Evidence
- Contextual Evidence

These types are not necessarily mutually exclusive. Contradiction is also relational: an item may support one Claim and contradict another.

Candidate Evidence-to-Claim relationship types:

- Supports
- Contradicts
- Qualifies
- Contextualizes
- Does Not Address

The relationship type must be distinguished from the assessment status. Candidate claim-specific statuses:

- Not Assessed
- Under Assessment
- Usable for Claim
- Usable with Restrictions
- Insufficient for Claim
- Not Applicable to Claim
- Conflicted for Claim
- Rejected for Specific Claim

Evidence must not receive a global Valid / Invalid label that silently applies to every possible use. Usability is Claim- and purpose-dependent.

### 17.9 Derived Evidence constraint

Derived Evidence may be produced through analysis, aggregation, transformation, or model-assisted processing. Its lineage must include all materially contributing Inputs and transformations.

A derived output must not be presented as an independent source merely because a tool or model generated it. New inferences introduced during processing must be distinguishable from information directly recorded in source material.

Derived Evidence is not necessarily weaker than Direct Evidence. A valid transformation may expose structure not readily observable in raw material. Its evidential use nevertheless depends on the method, assumptions, validation, provenance, and limitations being assessable.

### 17.10 Claim-specific sufficiency and coverage

Evidence reliability does not establish Claim sufficiency. A reliable operational log may support that an operation occurred while being insufficient to establish authorization for that operation.

For each Claim, assessment should consider:

1. Whether relevant Evidence exists.
2. Whether source attribution is sufficiently established.
3. Whether content integrity is adequate for the intended use.
4. Whether extraction fidelity is adequate.
5. Whether the Evidence applies to the defined Claim and Activity.
6. Whether required relationships among evidence items are established.
7. Whether material contradictory evidence or limitations remain.
8. Whether the total evidence set is sufficient under the applicable criteria.

Evidence Coverage remains claim-dependent and is not measured by document count. Relational Sufficiency remains distinct from the mere presence of multiple records.

### 17.11 Evidence lifecycle and preservation

Evidence lifecycle states are provisional and application-dependent:

- Candidate
- Under Assessment
- Assessed
- Usable for Specific Claim
- Restricted
- Challenged
- Rejected for Specific Claim
- Superseded
- Retracted

The status must identify the relevant Claim or evidential use where necessary. These states do not establish that an Evidence Object is universally valid or invalid.

Distinguish:

- **Evidence Correction:** an error in extraction, representation, or recorded content is corrected.
- **Evidence Retraction:** reliance on an Evidence Object is withdrawn or challenged.
- **Evidence Supersession:** a later version replaces an earlier one for a defined use.

Prior versions, source Inputs, transformation history, and previous Claim relationships must be preserved. Retraction does not prove the opposite proposition. A change in Evidence status triggers dependency-based impact review; it does not automatically reverse a Finding.

### 17.12 Evidence model invariants

- **ED-INV-01 — Entity Separation:** Input, Extracted Information, and Evidence remain distinct entities.
- **ED-INV-02 — No Automatic Evidential Promotion:** extraction alone does not establish Evidence validity or Claim support.
- **ED-INV-03 — Source Lineage Preservation:** each Evidence Object remains traceable to its source Inputs and relevant source locations.
- **ED-INV-04 — Transformation Transparency:** transformations, tools, versions, parameters, and known limitations are recorded.
- **ED-INV-05 — No Assumed Source Independence:** multiple sources are not presumed independent or corroborative by count alone.
- **ED-INV-06 — Claim-Specific Usability:** Evidence usability and sufficiency are assessed for a defined Claim and purpose.
- **ED-INV-07 — Proposition / Claim Separation:** Evidence Proposition, Claim, and Finding are not conflated.
- **ED-INV-08 — Derived Evidence Lineage:** derived outputs retain all materially contributing source and transformation references.
- **ED-INV-09 — Historical Evidence Preservation:** correction, retraction, and supersession preserve prior records and relationships.
- **ED-INV-10 — Dependency-Bounded Impact:** Evidence changes affect only elements connected through established and relevant dependencies.

### 17.13 Evidence extraction test matrix

| Test | Input / condition | Expected behavior |
|---|---|---|
| EX-T01 | PDF with extractable text | Preserve source and extracted text as separate objects. |
| EX-T02 | Scanned PDF processed by OCR | Record OCR method, version, source location, and fidelity limitations. |
| EX-T03 | Translation of a source document | Preserve original text and separately identify the translation. |
| EX-T04 | AI-generated summary | Distinguish source content from omissions and model-introduced inferences. |
| EX-T05 | One Input containing multiple propositions | Create separately identifiable extracted items with shared source lineage. |
| EX-T06 | Multiple Inputs contributing to one Evidence item | Preserve each source's contribution and dependency. |
| EX-T07 | Two reports with a common underlying source | Do not assume independent corroboration. |
| EX-T08 | Reliable Evidence unrelated to a Claim | Do not use it to support that Claim. |
| EX-T09 | Conflicting Evidence | Record conflict; do not automatically select one item. |
| EX-T10 | Corrected extraction | Preserve prior extraction and create a traceable corrected version. |
| EX-T11 | Evidence retraction | Review dependent Claims without automatic Finding reversal. |
| EX-T12 | Derived Evidence from multiple logs | Preserve all materially contributing source and transformation lineage. |
| EX-T13 | Authentic Input with no established Claim applicability | Preserve Input and extraction; do not change Claim Findings. |

### 17.14 EU-S-01 integrated test

For the fictional CV-ranking and automated-archiving scenario:

- A delegation PDF is Input I-01. Its extracted text is X-01. Evidence E-01 may be assessed for C1 and, if its content and scope support it, C2 or C3. Receipt of the document does not establish the authority chain, scope, or temporal validity.
- A ranking log is Input I-02 and may support E-02 for C5, subject to system and Activity linkage.
- An archive log is Input I-03 and may support E-03 for C6, subject to the same type of linkage.
- Operational configuration is Input I-04 and may be assessed for relevant scope and system relationships. It does not by itself establish authorization.
- A model-generated report describing a relationship between ranking and archiving is Derived Information. It is not independent proof of C7. The underlying event and transaction relationships must be established.
- An OCR or translation defect should affect only Evidence and Claims connected through established dependencies.

No evidence item or extraction event automatically establishes a Finding or changes unrelated Claim states.

---

## 18. Working architectural decisions — Evidence Object Model

**Decision status:** Proposed working architectural decisions for the Experimental Engineering Model. These are not Founder-approved program-level decisions, not validated requirements, and not BAES Foundation changes.

| ID | Proposed decision | Rationale / boundary |
|---|---|---|
| ED-01 | Keep Input, Extracted Information, and Evidence as three distinct entities. | Preserves separation between source, extracted content, and claim-specific evidential use. |
| ED-02 | Extraction alone must not promote information to valid or established Evidence. | Prevents extraction from being mistaken for source verification, applicability, or sufficiency. |
| ED-03 | Every extraction must retain source location and transformation lineage. | Enables provenance review and identification of lossy or error-prone transformations. |
| ED-04 | An Evidence Object may be supported by one or multiple Inputs. | Supports composite and multi-source evidence without collapsing source identity. |
| ED-05 | Source independence must not be inferred from source count. | Prevents false corroboration when records share an underlying source or production dependency. |
| ED-06 | Evidence applicability and sufficiency must be Claim- and purpose-dependent. | A source may be usable for one Claim and insufficient or irrelevant for another. |
| ED-07 | Evidence Proposition, Claim, and Finding must remain distinct. | Prevents source content from being silently converted into an assessment conclusion. |
| ED-08 | Derived Evidence must preserve all materially contributing sources and transformations. | Prevents model-generated or transformed outputs from acquiring unsupported evidential authority. |
| ED-09 | Evidence correction, retraction, and supersession must preserve historical versions and relationships. | Supports historical reconstruction and controlled reassessment. |
| ED-10 | Evidence changes may affect only Claims and assessment elements connected through established, relevant dependencies. | Enforces bounded impact and prevents uncertainty or change over-propagation. |

### 18.1 Decision application and change control

These decisions apply only to the current Experimental Engineering Model Working Design. They do not alter the frozen BAES Foundation, establish a new BAES requirement, or authorize publication of confidential BAES material.

They remain open to revision through explicit design review and test evidence. Any later change should preserve the previous decision wording, record the reason for change, and assess downstream effects through established dependencies.

### 18.2 Governing dependency principle

The following principle remains controlling:

> Uncertainty must be propagated according to established dependencies, not assumed associations.

It applies to source lineage, Evidence-to-Claim mapping, multi-source aggregation, conflict handling, and reassessment impact.

---

## 19. Next design stage: Evidence Aggregation and Conflict Resolution

The next open design task is to define how multiple Evidence Objects are assessed together for a Claim without relying on document counts, majority voting, assumed source independence, or generic numerical weights.

The next stage should distinguish Evidence Convergence, Corroboration, Conflict, Source Independence, Claim-specific evidential relevance, and any criteria-based assessment of evidential importance. It should define how conjunctive, disjunctive, and conditional Claim structures affect evidence aggregation, and how unresolved conflicts constrain Findings.

This stage remains open. No universal evidence-weighting formula or automatic conflict-resolution authority is established by the current design.

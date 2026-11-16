# BAES-EEM-TD-PILOT-001 — v0.1

Status: **Under Validation**. This is a constructed pilot dataset, not an empirically validated benchmark.

## Fixtures
- AT-01 — Ten Documents vs One Independent Source (variants A and B)
- AT-04 — Official but Irrelevant Document
- AT-13 — New but Unrelated Evidence

## Information separation
- `model-input*.json`: Model-visible scenario input.
- `assessment-package.json`, `claims.json`, `evidence.json`, `criteria.json`, `evidence-claim-assessments.json`, `model-available-dependency-graph.json`: model-side assessment material; use only the model-available graph.
- `reference-only.json`: evaluator-only ground truth and reference graph. Never pass to the model.
- `expected-behaviors.json`: evaluator-only expected behavior. Never pass to the model.
- `perturbations.json`: evaluator-controlled changes.

## Schema
JSON Schema Draft 2020-12 files are in `schemas/`. The schemas cover Dataset, Test Case, Fixture, Input Package, Reference Package, Assessment Package, Expected Behavior, Test Run, Evaluation Record, Activity, Claim, Criteria, Evidence, Evidence-Claim Assessment, Dependency Graph, Source Lineage Assessment, Conflict Record, Event, and State Transition.

## Validation status
Structural schema validation and selected cross-object checks are reported in `validation/`. Controls not executed or not fully implemented are explicitly marked accordingly. No model was selected or executed. No GitHub repository was modified.

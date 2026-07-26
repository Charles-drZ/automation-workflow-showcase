[← Automation workflow case study](../README.md)

# Architecture

The private workflow separates evidence collection, target observation, candidate preparation, review, and verification. This public page describes the responsibility boundaries without publishing the executable workflow.

## 1. Observe work evidence

Approved issue-tracker and Git sources are collected independently. Each source must be complete enough for review before it can influence a durable-memory candidate.

## 2. Observe current project memory

Existing durable documentation is inspected as a separate target state. Source evidence and target memory are not treated as interchangeable proof.

## 3. Validate integrity

Completeness, duplicate observations, malformed data, and uncertain joins are checked before interpretation. Material uncertainty stops the handoff rather than producing a confident-looking result.

## 4. Prepare deterministic candidates

Reproducible rules identify which observations may require review. This narrows the work before any optional model-assisted interpretation.

## 5. Build bounded review context

Only selected candidates receive minimized review context. Missing or truncated evidence remains visible to the reviewer.

## 6. Keep change authority human

Automation can prepare a proposal, but a human decides whether the project meaning is accurate, appropriately scoped, and safe to retain. Accepted changes follow normal repository review.

## 7. Verify the durable result

After an approved change is merged, the target is observed again. The workflow records the reviewed result only after the expected durable state is confirmed.

Exact contracts, field definitions, algorithms, prompts, node wiring, and synchronization records remain private.

---

[← Return to automation workflow case study](../README.md)

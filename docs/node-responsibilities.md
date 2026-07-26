[← Automation workflow case study](../README.md)

# Node-group responsibilities

This page describes conceptual responsibility groups. It is not a node-by-node export of the private n8n workflow.

## Trigger and coordination

Starts a manual or scheduled review cycle and keeps the major stages ordered.

## Source observation

Collects approved work and Git evidence through configured credentials and bounded source queries.

## Target observation

Inspects the current durable project-memory state separately from the work sources.

## Integrity gate

Checks whether the required observations are complete, unambiguous, and safe to compare. Material uncertainty stops the handoff.

## Deterministic candidate preparation

Applies reproducible selection rules to identify topics that may require review.

## Bounded context preparation

Minimizes the evidence supplied for selected candidates and keeps missing or truncated context visible.

## Structured review support

May use constrained model-assisted processing to help summarize or compare a candidate. It does not make the final project decision.

## Proposal preparation

Formats a reviewable change proposal without writing directly to a protected branch or declaring project work complete.

## Verification and reviewed state

Observes the durable result after an approved merge and records a reviewed synchronization outcome.

Exact node configuration, credential mapping, expressions, field contracts, prompts, endpoints, and wiring remain private.

---

[← Return to automation workflow case study](../README.md)

[← Automation workflow case study](../README.md)

# Data flow

The public model describes categories and decision boundaries, not the private workflow contract.

## Generic inputs

**Accepted work observation**  
Selected issue-tracker evidence describing completed or reviewable work.

**Git evidence observation**  
Selected repository evidence showing that relevant implementation work exists.

**Durable-memory observation**  
The current reviewed project-memory state for the same topic.

**Integrity state**  
Whether required source coverage is complete and unambiguous enough to continue.

## Generic processing

1. Observe each source independently.
2. Validate completeness and integrity.
3. Compare work evidence with the current durable-memory state.
4. Prepare deterministic review candidates.
5. Build minimized context only for selected candidates.
6. Keep the final decision and change approval human-controlled.

## Generic outputs

**Validated observation set**  
A traceable view of the evidence categories considered for the review cycle.

**Review candidate**  
A topic that may need clarification, durable documentation, or no action.

**Bounded review context**  
A minimized package for human-led or model-assisted interpretation.

**Approved proposal**  
A reviewed change prepared for normal repository review rather than a direct protected-branch write.

**Verified durable result**  
Confirmation that the accepted project-memory state exists after merge.

Real payloads, exact fields, schemas, source identifiers, private responses, and synchronization records are intentionally excluded.

---

[← Return to automation workflow case study](../README.md)

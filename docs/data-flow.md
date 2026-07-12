# Data flow

## Generic inputs

| Input | Normalized fields |
| --- | --- |
| Commit activity | Source, short summary, change category, review relevance |
| Work item | Status, accepted scope summary, validation state, relevance |
| Existing memory signal | Topic, last-known context, update candidate |

## Generic outputs

| Output | Purpose |
| --- | --- |
| Deterministic digest | A traceable view of selected input before interpretation. |
| Structured summary | Optional concise interpretation using constrained fields. |
| Sync candidate | A proposed durable-memory update awaiting review. |

Inputs are selected and minimized for the task. Real payloads, live responses, internal URLs, and personal information are intentionally excluded from this public repository.

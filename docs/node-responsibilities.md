# Node responsibilities

| Generic node | Responsibility |
| --- | --- |
| Trigger | Starts a manual or scheduled run. |
| HTTP request | Retrieves an approved external source through configured credentials. |
| GitHub source | Collects selected commit metadata. |
| Linear source | Collects selected issue metadata. |
| Code node | Normalizes fields and applies deterministic selection rules. |
| Merge | Combines normalized branches once their inputs are ready. |
| Digest | Builds a concise, deterministic review input. |
| OpenAI | Optionally produces a structured summary from the digest. |
| Output preparation | Formats a reviewable candidate without performing an unreviewed durable write. |

The exact node configuration, credential mapping, and live endpoints are private.

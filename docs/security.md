[← Automation workflow case study](../README.md)

# Security and publication boundary

- Credentials remain in the private automation environment rather than public workflow content.
- Tokens, authorization headers, webhooks, endpoints, and private responses are excluded.
- Source access follows least-privilege and read-only principles where possible.
- Real issue bodies, repository payloads, execution data, prompts, and durable-memory documents are not copied into this repository.
- Public examples are synthetic and contain no real people, repositories, commit identifiers, issue identifiers, or operational configuration.
- Incomplete or uncertain evidence blocks a durable handoff instead of producing a confident-looking result.
- A human approves project meaning, privacy, and any proposed durable update.
- Approved changes use normal repository review rather than an unreviewed direct write to a protected branch.

These practices make the case study useful without publishing the operational workflow or weakening the private project boundary.

---

[← Return to automation workflow case study](../README.md)

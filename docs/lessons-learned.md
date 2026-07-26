[← Automation workflow case study](../README.md)

# Lessons learned

- Keep work evidence and current durable-memory observations separate until comparison is intentional.
- Treat pagination, enrichment, duplicate keys, and malformed artifacts as integrity concerns rather than implementation trivia.
- Apply deterministic selection before optional semantic interpretation.
- Fail closed when source coverage or joins are uncertain.
- Build bounded review context only for selected candidates.
- Preserve visible evidence of truncation or missing context.
- Let automation prepare proposals, not decide product meaning or completion.
- Verify the durable result after merge instead of assuming an accepted proposal became correct project memory.
- Use n8n credential handling and least-privilege source access deliberately.
- Keep model context and cost bounded by minimizing inputs before review.

The strongest automation is not the one that writes the most. It is the one that makes uncertainty visible and keeps consequential decisions reviewable.

---

[← Return to automation workflow case study](../README.md)

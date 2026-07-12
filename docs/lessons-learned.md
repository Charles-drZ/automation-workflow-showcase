# Lessons learned

- Avoid accidental fan-out: independent source branches should not cause repeated downstream execution.
- Normalize before merge so comparisons and selection rules stay predictable.
- Build a deterministic digest before optional AI processing.
- Separate source collection from interpretation.
- Review a candidate before writing durable memory.
- Use expression mode and credential handling deliberately in n8n.
- Keep token cost in view by sending only the context needed for the task.
- Do not treat an AI summary as the authoritative project record without review.

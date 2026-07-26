[← Automation workflow case study](../README.md)

# Visual publication plan

Visual evidence is added only after the relevant private workflow surface is stable and the proposed image has passed a separate privacy and reconstructability review.

The goal is to show system thinking, responsibility boundaries, and evidence flow. It is **not** to publish the private n8n implementation, exact node wiring, contracts, prompts, payloads, or operational configuration.

## Planned visual set

1. **`visuals/01-workflow-overview.png` — Sanitized workflow overview**  
   Show the major workflow regions at a readable zoom using generalized labels. The image should communicate observation, integrity checking, candidate preparation, human review, and verification without exposing exact nodes or expressions.

2. **`visuals/02-source-and-target-observation.png` — Observation boundaries**  
   Show that work evidence, Git evidence, and durable-memory observations remain distinct before comparison. Use generic group labels and no live source data.

3. **`visuals/03-integrity-and-candidate-flow.png` — Integrity gate and candidate preparation**  
   Show the fail-closed boundary and the transition from validated observations to bounded review candidates. Do not reveal matching keys, canonicalization rules, fingerprints, schemas, or branching expressions.

4. **`visuals/04-human-review-gate.png` — Human decision boundary**  
   Show where semantic review and publication authority remain human-controlled. No private review text, prompt, issue content, or automatic write instruction may be visible.

5. **`visuals/05-verification-loop.png` — Post-change verification**  
   Show that an approved change follows normal repository review and is observed again before a reviewed synchronization state is recorded. Keep repository paths, branch names, identifiers, and record structure private.

6. **`visuals/06-synthetic-review-candidate.png` — Optional synthetic example**  
   Use only invented content that explains why a candidate requires human review. It must not imitate a private payload or reproduce the real contract shape.

## Capture and redrawing guidance

- Prefer a purpose-built sanitized export or redrawn overview over a raw production screenshot.
- Use consistent zoom, crop, typography, and image dimensions across the set.
- Hide the n8n sidebar, execution history, browser tabs, account information, environment labels, and notification surfaces.
- Replace internal node names with generalized public labels where revealing the real name would expose implementation structure.
- Use synthetic sample values only. Do not blur real private text when it can be removed or replaced before capture.
- Keep credentials, expressions, code editors, input/output inspectors, execution data, and error payloads closed.
- Export as PNG or WebP. Do not publish raw HEIC captures, animated GIFs, SVGs containing editable text, or HTML exports.
- Remove image metadata before publication and review the final exported file, not only the source canvas.

## Never include

- credentials, tokens, authorization headers, webhook URLs, endpoints, or account details;
- real issue descriptions, comments, ticket identifiers, execution identifiers, timestamps, or live counts;
- private repository paths, branch names, commit identifiers, file names, or project-memory document names;
- exact node configuration, expressions, JavaScript, workflow JSON, input/output payloads, or API responses;
- contract fields, schemas, canonicalization rules, fingerprint inputs, ledger structure, or idempotency keys;
- model prompts, private review packets, automatic write instructions, or unreviewed durable-memory text;
- GlassBox source code, source excerpts, implementation evidence, or unreleased product information;
- personal data, browser profile information, local paths, or machine-specific details.

## Pre-publication checklist

- [ ] The visual proves a specific recruiter-facing claim that is already supported by the written case study.
- [ ] The image uses generalized or synthetic labels rather than private implementation names.
- [ ] No credential, endpoint, identifier, payload, prompt, source excerpt, execution detail, or real issue content is visible.
- [ ] The visual cannot be used to reconstruct the private workflow or its contracts.
- [ ] Browser chrome, account details, notifications, local paths, and environment names are absent.
- [ ] The crop and zoom are readable on both desktop and mobile GitHub views.
- [ ] Image metadata has been removed and the exported file has been reviewed separately.
- [ ] The README caption accurately describes what the image proves and what remains private.
- [ ] Final publication approval has been given by the repository owner.

---

[← Return to automation workflow case study](../README.md)

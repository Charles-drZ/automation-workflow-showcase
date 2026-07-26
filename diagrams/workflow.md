[← Automation workflow case study](../README.md)

# Workflow diagram

```mermaid
flowchart TD
    A[Manual or scheduled review cycle] --> B[Work-source observation]
    A --> C[Git-evidence observation]
    A --> D[Durable-memory observation]
    B --> E[Integrity and completeness gate]
    C --> E
    D --> E
    E -->|uncertain| F[Fail closed and report evidence gap]
    E -->|complete| G[Deterministic candidate preparation]
    G --> H[Bounded review context]
    H --> I[Human-led semantic review]
    I --> J[Review-gated change proposal]
    J --> K[Normal repository review and merge]
    K --> L[Observe and verify durable result]
    L --> M[Record reviewed synchronization state]
```

The workflow is deliberately staged: observe independently, validate integrity, narrow candidates deterministically, review meaning under human control, and verify the durable result after merge.

The diagram is conceptual. Exact source contracts, node wiring, prompts, proposal format, and synchronization records remain private.

---

[← Return to automation workflow case study](../README.md)

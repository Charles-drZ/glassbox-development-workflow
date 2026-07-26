[← Development workflow case study](../README.md)

# Source-of-truth model

No single tool is the answer to every project question. The workflow assigns each system a purpose so information stays reviewable and does not drift.

```mermaid
flowchart TD
    X[Codex: bounded audit and implementation] --> G[GitHub: committed implementation evidence]
    N[n8n: deterministic preparation] --> B[Brainflow: durable memory and decisions]
    L[Linear: current scope and status] --> H[Human review]
    G --> H
    B --> H
    C[ChatGPT: orchestration and review] --> H
    H --> L
```

## What each source answers

**Linear**  
What is currently accepted, in scope, and under review?

**GitHub**  
What was committed and when?

**Brainflow**  
What durable decisions, summaries, and historical context matter?

**ChatGPT**  
How should an idea be shaped, reviewed, or evaluated?

**Codex**  
What did a bounded audit or implementation find and validate?

**n8n**  
How can selected information be processed and prepared consistently?

**Human reviewer**  
What is approved for implementation, release, privacy, and publication?

The model is intentionally human-controlled. Tool outputs assist decisions; they do not silently replace them.

---

[← Return to development workflow case study](../README.md)

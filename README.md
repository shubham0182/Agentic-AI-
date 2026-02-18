## 🧭 Agentic AI Workflow Diagram

The following diagram explains how the Agentic AI workflow operates inside **:contentReference[oaicite:0]{index=0}**, from input to autonomous task execution.

```mermaid
flowchart TD
    A[Trigger<br/>(Webhook / Schedule / User Input)]
    B[AI Agent<br/>Reasoning & Planning]
    C{Decision Node}
    D[Execute Tool<br/>(API / Script / Service)]
    E[Evaluate Result]
    F{Goal Achieved?}
    G[End Workflow]
    H[Refine Prompt / Retry]

    A --> B
    B --> C
    C -->|Yes| D
    D --> E
    E --> F
    F -->|Yes| G
    F -->|No| H
    H --> B

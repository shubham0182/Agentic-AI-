## 🧭 Agentic AI Workflow Diagram

The diagram below explains the Agentic AI workflow implemented using **:contentReference[oaicite:0]{index=0}**.

```mermaid
flowchart TD
    A[Trigger: Webhook or Schedule or User Input]
    B[AI Agent Reasoning and Planning]
    C{Decision Logic}
    D[Execute Tool or API]
    E[Evaluate Result]
    F{Goal Achieved}
    G[End Workflow]
    H[Refine Prompt and Retry]

    A --> B
    B --> C
    C -->|Proceed| D
    D --> E
    E --> F
    F -->|Yes| G
    F -->|No| H
    H --> B

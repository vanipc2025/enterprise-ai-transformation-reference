# Enterprise AI Reference Architecture — CGOATKMM

This is a reasoning aid, not a requirement to deploy eight layers.

```mermaid
flowchart TD
 C[Channels<br/>people • apps • APIs • devices] --> G[Gateway<br/>identity • policy • routing • filtering]
 G --> O[Orchestration<br/>workflow • planning • approvals • state]
 O --> A[Agents<br/>bounded autonomous actors]
 A --> T[Tools<br/>APIs • enterprise apps • databases • devices]
 A --> K[Knowledge<br/>RAG • search • graph • enterprise content]
 A --> MM[Memory<br/>session • working • persistent state]
 O --> M[Models<br/>ML • LLM • SLM • multimodal • specialist]
 K --> M
 MM --> M
```

## SGOE surrounds the stack
**Security** protects identities, data, models, agents, tools and infrastructure.  
**Governance** defines accountability, policy, risk tolerance and human authority.  
**Observability** exposes prompts, retrieval, tool calls, latency, failures and cost.  
**Evaluation** measures quality, grounding, task success, safety and business outcomes.

## Rule
Start with the minimum required layers. Increase autonomy only when its expected value exceeds the added operational and security risk.

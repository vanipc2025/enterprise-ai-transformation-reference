# Architecture Decisions & Trade-offs

Architecture quality is demonstrated by **why a choice was made**, not by how many technologies appear in a diagram.

## Core decision set

| Decision | Main tension |
|---|---|
| Conventional software vs AI | determinism vs probabilistic capability |
| Traditional ML vs GenAI | prediction vs generation/reasoning |
| RAG vs fine-tuning | runtime knowledge vs behavior specialization |
| Workflow vs agent | predictability vs autonomy/adaptivity |
| Single vs multi-agent | simplicity vs specialization/coordination |
| LLM vs SLM/specialist | breadth vs latency/cost/control |
| One model vs routing | simplicity vs workload optimization |
| Edge vs cloud | latency/privacy/connectivity vs scale/operations |
| API vs agent/tool protocol | explicit integration vs dynamic tool discovery/use |
| Human approval vs autonomy | speed vs consequence/control |
| Build vs buy | differentiation/control vs speed/operational burden |

Every decision record should capture context, options, decision, rationale, consequences, SGOE controls, economics and evidence to revisit the decision.

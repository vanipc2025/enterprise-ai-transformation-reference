# Models — the Intelligence Layer

A model is one component of an enterprise AI system, not the architecture itself.

## Model classes an architect may combine

| Class | Useful for | Key trade-offs |
|---|---|---|
| Traditional ML | prediction/classification on structured signals | strong task focus; requires appropriate features/data |
| Embedding model | semantic retrieval and similarity | retrieval quality, language/domain fit, cost |
| LLM | language understanding/generation and broad tasks | capability vs latency/cost/control |
| SLM | bounded tasks, edge/private/low-latency cases | efficiency vs breadth/capability |
| Reasoning model | complex multi-step problems | higher latency/cost; evaluation essential |
| Multimodal model | text + image/audio/video inputs | richer capability, larger data/privacy surface |
| Specialist model | vision, speech, forecasting, anomaly detection etc. | excellent task fit; integration complexity |

## Selection criteria

Choose against the workload: **quality, task success, grounding, latency, throughput, context need, privacy, residency, deployment model, safety, explainability, integration, availability and unit cost**.

Parameter count alone is not an enterprise selection strategy. Larger models can improve some capabilities but may increase latency and cost. Smaller/specialist models can be better for bounded tasks.

## Improve accuracy in the right place

Before fine-tuning, identify the failure source:

`source data → retrieval → context → prompt/instructions → model capability → tool output → orchestration → human/process`

Use RAG for changing/external enterprise knowledge; prompting for instructions; fine-tuning when behavior/task specialization warrants it; model routing when different tasks justify different capability/cost profiles.

## Production principle

Evaluate models on the organization's own representative tasks and failure conditions. Benchmark scores are inputs, not proof that the complete enterprise system works.

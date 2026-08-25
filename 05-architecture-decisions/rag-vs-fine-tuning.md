# RAG vs Fine-Tuning

Do not use fine-tuning as the default answer to poor factual accuracy.

| Need | Investigate first |
|---|---|
| Frequently changing enterprise facts | Retrieval / RAG |
| Private policies/documents | Retrieval / RAG |
| Consistent style or behavior | Prompting or fine-tuning |
| Specialized task behavior | Fine-tuning may help |
| Missing/poor source data | Fix the data |
| Poor retrieval | Chunking, metadata, search, reranking, evaluation |
| General reasoning limitation | Model selection/routing |

Fine-tuning primarily changes model behavior; retrieval supplies external knowledge at runtime. They can be combined.

Diagnose whether an error originates in **data, retrieval, context, prompt, model, tool result or workflow** before changing model parameters.

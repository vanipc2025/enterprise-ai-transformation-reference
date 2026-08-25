# Applications & Legacy Architecture

Legacy does not simply mean old. A system becomes a transformation constraint when its interfaces, data, changeability, security, economics or operational coupling prevent the required business outcome.

## Typical issues

| Legacy issue | Transformation consequence | Possible disposition |
|---|---|---|
| Monolith / mainframe dependency | slow change, tightly coupled workflows | retain + expose, strangler modernization, selective replacement |
| ERP/CRM customization | upgrades and integrations become expensive | retain core, rationalize customization, API/service facade |
| Batch/file interfaces | stale context and weak agent interaction | retain where sufficient; add APIs/events for priority flows |
| Undocumented interfaces | migration and tool-call risk | discover, contract-test, document, wrap |
| Data silos / duplicate masters | poor retrieval and inconsistent decisions | ownership, canonical data, governed access |
| Weak identity boundaries | AI may over-access systems/data | modern identity, workload/agent identity, least privilege |
| Knowledge in PDFs/email | experts spend time searching/reconciling | governed knowledge pipeline/RAG where appropriate |
| Unsupported technology | security and continuity risk | isolate, upgrade, replatform or replace |

## Disposition vocabulary

**Retain • Wrap • Integrate • Replatform • Refactor • Replace • Retire**

The consultant should decide component by component. A wholesale rewrite can be as risky as indefinitely wrapping everything.

## AI-specific warning

Do not give an agent broad tool access merely because a legacy system lacks granular APIs. The modernization work may need to create safe, task-scoped interfaces before autonomy is introduced.

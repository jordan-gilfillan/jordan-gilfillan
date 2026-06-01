# Hi, I'm Jordan Gilfillan 👋

**AI Systems Engineer · Principal Consultant.** I build practical LLM and retrieval systems — ingestion → representation → retrieval → guarded generation → tests — and the evaluation harnesses that keep them honest.

🌐 [jordangilfillan.com](https://jordangilfillan.com)  ·  📧 jordan@jordangilfillan.com

---

## What I'm building now

### Throughline — synthesis and retrieval over your own AI conversation history

Throughline turns AI conversation exports (ChatGPT, Claude, Grok, Gemini) into a queryable, longitudinal record of your *own* writing. It imports exports into a common schema, extracts only user-authored messages, synthesizes first-person daily journal entries that cite back to the source messages, embeds them for semantic search, and presents the whole corpus through a local web UI — browse by date, by similarity, and on a 2D map where related entries cluster.

**Design commitments**

- **Single-tenant by design** — you run it yourself with your own API key; nothing is pooled through an operator's backend. Synthesis and embeddings call OpenAI in v1 (fully local models are planned, not yet shipped).
- **Provenance preserved** — every synthesized entry cites the exact messages it came from, and the synthesis prompt forbids invention.
- **Artifacts, not a chatbot** — it produces things you read and act on, not another conversation.
- **Tested behavior** — 94 tests cover the parsers, sanitizer, day-grouping, embedding cache, and search ranking.

**Stack:** Python · OpenAI · UMAP · Streamlit · pytest

**Status:** v1, pre-release. The pipeline runs end to end on sample data (import → synthesize → embed → browse / search / visualize). A public demo is in progress.

---

## How I work (spec-first)

Before I optimize anything, I write down:

1. **Bottleneck** — what's actually limiting the outcome
2. **Spec** — behavior that can be tested
3. **Lever** — the smallest change that moves the bottleneck

And I hold the work to three things: **invariants** (what must stay true), **acceptance criteria** (what "done" means), and a **not-doing list** (scope control).

---

## What I'm good at

- **Embeddings + retrieval** — chunking strategies, vector search, hybrid retrieval when it earns its place
- **RAG that ships** — guardrails, citations, traceability, and evaluation harnesses instead of vibes
- **Pragmatic systems** — Python + TypeScript/Node glue, clean APIs, CI, tests, reproducibility
- **Privacy-minded design** — single-tenant architecture, explicit access decisions, auditable behavior

---

## Working together

Available for **selective consulting** on AI systems — RAG and retrieval, evaluation and quality harnesses, data pipelines for unstructured text, and pragmatic engineering for teams that need systems to actually hold up in production.

Also open to the right **full-time role** where shipping reliable applied-AI systems is the point.

📧 jordan@jordangilfillan.com  ·  🌐 [jordangilfillan.com](https://jordangilfillan.com)

---

## Contact

- **Email** — jordan@jordangilfillan.com
- **Web** — [jordangilfillan.com](https://jordangilfillan.com)
- **GitHub** — [github.com/jordan-gilfillan](https://github.com/jordan-gilfillan)

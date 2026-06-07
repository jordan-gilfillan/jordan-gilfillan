# Hi, I'm Jordan Gilfillan 👋

**AI Systems Engineer · Principal Consultant.** I build practical LLM and retrieval systems — ingestion → representation → retrieval → guarded generation → tests — and the evaluation harnesses that keep them honest.

🌐 [jordangilfillan.com](https://jordangilfillan.com)  ·  📧 jordan@jordangilfillan.com

---

## What I'm building now

### Inscape — a privacy-gated, queryable mirror of a person, built from their own AI conversations

Inscape turns years of AI-chat history into a queryable model of how someone thinks — and gates every answer by the *relationship* of the person asking. The same system shows a professional contact the professional view, a friend more, and the owner everything; the boundary is enforced server-side and stress-tested, and every answer cites the real entries it's grounded in. The privacy model isn't a wrapper around the demo — it *is* the demo: context-appropriate disclosure, the way people actually relate.

**Highlights**

- **Relationship-aware privacy** — an access code maps to a policy, enforced through a layered pipeline (refuse the question → filter the evidence → filter the output) that's derived server-side, never from the client.
- **Provenance preserved** — answers cite the exact source entries; synthesis is constrained to the person's own words and forbidden from inventing.
- **Tested boundaries** — a full test suite plus an adversarial over/under-share eval (deterministic checks + an LLM judge) that I used to find and close real oversharing leaks.
- **Built solo by directing coding models** — I designed the architecture and the privacy model, wrote the eval, and traced and fixed the failures.

**Stack:** Next.js · TypeScript · SQLite + embeddings · OpenAI

**Status:** v1, launching as an invite-gated live demo. More at [jordangilfillan.com](https://jordangilfillan.com).

### Throughline — synthesis and retrieval over your own AI conversation history

Throughline turns AI conversation exports (ChatGPT, Claude, Grok; Gemini planned) into a queryable, longitudinal record of your *own* writing. It imports exports into a common schema, extracts only user-authored messages, synthesizes first-person daily journal entries that cite back to the source messages, embeds them for semantic search, and presents the corpus through a local web UI — browse by date, by similarity, and on a 2D map where related entries cluster.

**Design commitments**

- **Single-tenant by design** — you run it yourself with your own API key; nothing is pooled through an operator's backend.
- **Provenance preserved** — every synthesized entry cites the messages it came from; the synthesis prompt forbids invention.
- **Artifacts, not a chatbot** — it produces things you read and act on.
- **Tested behavior** — 94 tests cover the parsers, sanitizer, day-grouping, embedding cache, and search ranking.

**Stack:** Python · OpenAI · UMAP · Streamlit · pytest

**Status:** v1, pre-release; runs end to end on bundled sample data with no API key. Open-source.

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
- **Privacy-minded design** — single-tenant architecture, server-enforced access decisions, auditable behavior
- **Pragmatic systems** — Python + TypeScript/Node glue, clean APIs, CI, tests, reproducibility

---

## Working together

Available for **selective consulting** on AI systems — RAG and retrieval, evaluation and quality harnesses, data pipelines for unstructured text, and pragmatic engineering for teams that need systems to hold up in production. Also open to the right **full-time role** where shipping reliable applied-AI systems is the point.

📧 jordan@jordangilfillan.com  ·  🌐 [jordangilfillan.com](https://jordangilfillan.com)  ·  💻 [github.com/jordan-gilfillan](https://github.com/jordan-gilfillan)

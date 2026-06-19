# Hi 👋 I build production agentic systems

I design and ship **AI agents that act safely in production** — and the
vertical software they live inside. Three years building with Claude / Claude
Code, with a focus on the hard part: letting autonomous systems *write* to real
data without breaking things.

🇫🇷 Based in **Paris, France** · 🗣️ FR / EN · available remote
<!-- Fill in: name, @handle, email, links you want public -->

---

## What I work on

**Safe agentic architecture.** I built an AI "chief of staff" embedded in a
production ERP: a layered design with tiered governance (auto / confirm /
human-approval), a human-in-the-loop gate on high-impact actions, and 20+
validated write-actions across the system. The interesting engineering is in the
*guardrails*, not the demo.

**Agentic engineering at scale.** An agentic development harness that generates,
gates and merges pull requests — with a 9-gate auto-merge pipeline, an
**independent-model review oracle**, a post-merge spot-audit, kill-switches and a
re-evaluation path — **400+ merged PRs** to date (26 gate-auto-merged behind the 9
gates; the rest human-reviewed). Backed by real **evals & observability**: golden
datasets, trajectory evals, per-agent-call tracing, and context-recall metrics.
Because "it works on my prompt" isn't production. *(The sanitized verdict core is
public — see `harness-demo` below.)*

**AI-native vertical ERP.** A multi-tenant SaaS ERP (**21 modules**,
FastAPI · Supabase · Pydantic v2) serving agri-businesses, with a **deployed ERP
chatbot passing a 20/20 golden-query suite**, internationalized across
**25,000+ translation keys in 4 locales**, over a **447-table schema with 446
tables RLS-enabled** — real deployment, real operations, real constraints.

**Applied ML on small data.** Gradient-boosted models (CatBoost / XGBoost) and
on-device inference (ONNX) for forecasting; a custom computer-vision pipeline
(YOLO) for field measurement from phone photos.

---

## Open source

| Repo | What it is |
|---|---|
| **harness-demo** | The fail-closed verdict core that lets an agent merge to prod *safely* — 9 gates + independent-model oracle + post-merge audit, 48 fixtures, runnable demo, honest "how it can still fail" |
| **agent-guardrails** | Tier 1/2/3 + HITL governance for agent write-actions — ~250 lines, zero deps |
| **langgraph-hitl-agent** | Runnable LangGraph agent that pauses on high-impact actions via `interrupt()` |
| **mcp-server-starter** | Real MCP server (FastMCP) with a destructive action guarded behind human confirmation |
| **fastapi-supabase-multitenant-starter** | Multi-tenant SaaS skeleton with Postgres RLS isolation |
| **claude-mcp-recipes** | Battle-tested MCP setups (Linear · Supabase · Sentry · Vercel) for a real Claude Code dev loop |

The core ERP business logic stays private — what's public is the reusable
engineering underneath it.

---

## Stack

`Python` · `FastAPI` · `Supabase / Postgres (RLS)` · `Pydantic v2` ·
`Claude / Claude Code` · `MCP` · `LangGraph` · `RAG` · `CatBoost / XGBoost` ·
`ONNX` · `YOLO` · `Linear` · `Vercel` · `Sentry`

---

## Open to

Architecture audits for agentic systems · designing safe agent write-flows ·
MCP server development · LangGraph / multi-agent systems with human oversight ·
RAG pipelines · Python backend for SaaS / ERP. A francophone, on-the-ground
understanding of African markets is a bonus where it's relevant.

<!-- 📫 Reach me: {{email}} · {{linkedin}} · {{malt / upwork}} -->

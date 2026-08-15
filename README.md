# Developer Roadmaps

Visual, interactive developer roadmaps — step-by-step guides for building modern AI & application systems, shared as clean, self-contained HTML artifacts. Each one is a single-file, interactive recreation in the spirit of the roadmap-style guides developers already love (à la roadmap.sh) — no build step, just open it in a browser.

**Live gallery:** https://fahdi.github.io/dev-roadmaps/

## Roadmaps

| Roadmap | Description |
|---|---|
| [AI Application Architecture](artifacts/ai-application-architecture.html) | Frontend → Agent Orchestration → Knowledge / Models / Tools → Data Layer → Observability & Evals → Deployment, plus the twelve-layer build order |
| [The Full AI Stack](artifacts/the-full-ai-stack.html) | LLMs → Embeddings → Vector DB → Extraction → Access → Frameworks → Evaluation. A newer model helps, better architecture helps more |
| [How to Build a RAG](artifacts/how-to-build-a-rag.html) | Load → Chunk → Embed & Tag → Index → Retrieve → Augment → Generate → Verify → Evaluate, plus the five moves every RAG buzzword belongs to |
| [RAG vs LoRA vs Full Fine-Tuning](artifacts/rag-vs-lora-vs-fine-tuning.html) | Context, adapters, or every weight — pick by the gap: knowledge → RAG, behavior → train |
| [Fine-Tune an LLM, End to End](artifacts/fine-tune-an-llm.html) | Curate examples → training data → full or adapter → SFT loop → gate on unseen splits → version, canary, monitor. Teach behaviour, retrieve facts |
| [Design Your Agent's Control Plane](artifacts/agent-control-plane.html) | CLAUDE.md → Rules → Skills → Agents → Hooks → Plugin — context tells, skills teach, agents delegate, hooks enforce, plugins ship the set |
| [6 Levels of Agentic AI](artifacts/six-levels-of-agentic-ai.html) | Basic → Router → Tool Calling → Multi-agent → Autonomous → Loop Engineering — levels 1–5 are capabilities, level 6 is the craft: discover, plan, execute, verify, iterate |
| [Context Engineering](artifacts/context-engineering.html) | The window is a budget: write, select, compress, isolate — the four memory stores, and the four failure modes of long context |
| [How a Request Travels](artifacts/how-a-request-travels.html) | DNS → TLS → CDN → Load Balancer → API Gateway → Service → Cache → Database — the two cache shortcuts, and what changes when the service is a model |
| [How to Evaluate an LLM App](artifacts/evaluating-llm-apps.html) | Evals measure, guardrails enforce, monitoring detects — golden dataset → four evaluators → six score dimensions → CI/CD gate → guardrails → online evals — failures become test cases |

## Structure

```
index.html             gallery landing page (published via GitHub Pages)
artifacts/*.html        one self-contained HTML roadmap per file
```

## Adding a new roadmap

1. Drop a new self-contained `.html` file into `artifacts/`.
2. Add a card for it to `index.html` and a row to the table above.
3. Commit and push — GitHub Pages redeploys automatically.

---

Built by [Fahad Murtaza](https://github.com/fahdi) with Claude.

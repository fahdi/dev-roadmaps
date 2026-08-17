# Developer Roadmaps

Visual, interactive developer roadmaps: step-by-step guides for building modern AI & application systems, shared as clean, self-contained HTML artifacts. Each one is a single-file, interactive recreation in the spirit of the roadmap-style guides developers already love (à la roadmap.sh). No build step, just open it in a browser.

**Live gallery:** https://fahdi.github.io/dev-roadmaps/

## Roadmaps

| Roadmap | Description |
|---|---|
| [AI Application Architecture](artifacts/ai-application-architecture.html) | Frontend → Agent Orchestration → Knowledge / Models / Tools → Data Layer → Observability & Evals → Deployment, plus the twelve-layer build order |
| [The Full AI Stack](artifacts/the-full-ai-stack.html) | LLMs → Embeddings → Vector DB → Extraction → Access → Frameworks → Evaluation. A newer model helps, better architecture helps more |
| [How to Build a RAG](artifacts/how-to-build-a-rag.html) | Load → Chunk → Embed & Tag → Index → Retrieve → Augment → Generate → Verify → Evaluate, plus the five moves every RAG buzzword belongs to |
| [RAG vs LoRA vs Full Fine-Tuning](artifacts/rag-vs-lora-vs-fine-tuning.html) | Context, adapters, or every weight. Pick by the gap: knowledge → RAG, behavior → train |
| [AI Model Lifecycle](artifacts/ai-model-lifecycle.html) | Training → fine-tuning → serving → inference. Four activities with different costs and owners, routinely used as synonyms |
| [Fine-Tune an LLM, End to End](artifacts/fine-tune-an-llm.html) | Curate examples → training data → full or adapter → SFT loop → gate on unseen splits → version, canary, monitor. Teach behaviour, retrieve facts |
| [Design Your Agent's Control Plane](artifacts/agent-control-plane.html) | CLAUDE.md → Rules → Skills → Agents → Hooks → Plugin. Context tells, skills teach, agents delegate, hooks enforce, plugins ship the set |
| [6 Levels of Agentic AI](artifacts/six-levels-of-agentic-ai.html) | Basic → Router → Tool Calling → Multi-agent → Autonomous → Loop Engineering. Levels 1-5 are capabilities, level 6 is the craft: discover, plan, execute, verify, iterate |
| [API vs Function Calling vs MCP](artifacts/api-function-calling-mcp.html) | Three layers of one stack, not competing options. API executes, function calling lets the model request, MCP standardises access |
| [The Agentic Loop](artifacts/the-agentic-loop.html) | Gather context → take action → verify → loop. Model reasons, tools act, harness orchestrates, and you can steer mid-run |
| [12 Prompt Patterns](artifacts/prompt-patterns.html) | Zero/one/few-shot → chain of thought, roles, self-reflection → structured output, delimiters, constraints → context selection, templates, prefix caching |
| [Context Engineering](artifacts/context-engineering.html) | The window is a budget: write, select, compress, isolate, the four memory stores, and the four failure modes of long context |
| [10 Interview Patterns, Animated](artifacts/interview-patterns.html) | Interactive. Two pointers through dynamic programming, each with a live mechanic and the recognition signal that selects it |
| [DSA: 24 Nodes in the Right Order](artifacts/dsa-roadmap.html) | Fundamentals → DP and graphs → specialised structures. Recursion at node six is the hinge, and DP is node eleven for a reason |
| [Build, Orchestrate, Observe](artifacts/langchain-langgraph-langsmith.html) | Component layer, control flow layer, visibility layer. Not alternatives, three different questions |
| [SQL: 24 Nodes to Production](artifacts/sql-roadmap.html) | Fundamentals → joins → window functions → EXPLAIN, indexes and transactions. Window functions are the jump |
| [Kafka in 12 Concepts](artifacts/kafka-concepts.html) | Producer → topic → partition → broker → consumer, plus offsets, replication, retention, schemas and Connect. The partition is the whole idea |
| [Distributing Data Across Nodes](artifacts/distributing-data.html) | Why modulo hashing breaks, the hash ring, virtual nodes, replication and quorums, then what CAP actually costs during a partition |
| [12 System Design Patterns](artifacts/system-design-patterns.html) | Timeout, retry, circuit breaker, rate limiter, bulkhead, pub/sub, caching, event sourcing, CQRS, saga, strangler fig. Every one is about failure |
| [API Security, Attack by Attack](artifacts/api-security.html) | Interactive. Broken object and function authorization, mass assignment, data exposure, unbounded consumption, SSRF and forgotten APIs, each with naive and hardened responses |
| [HTTPS and TLS, Watched Live](artifacts/https-tls.html) | Interactive. An eavesdropper captures the same packets either way, plus key exchange, certificates, metadata leakage and where the tunnel ends |
| [API Key vs JWT vs OAuth 2.0](artifacts/api-key-jwt-oauth.html) | App to app, user to app, user to third party. One product usually runs all three for different hops |
| [System Design Map](artifacts/system-design-map.html) | Twelve must-know designs and what each is really testing, from URL shorteners to agentic AI. Far fewer ideas than designs |
| [Demo to Production](artifacts/demo-to-production.html) | Interactive. Retrieval, agents, context, evals, failure, cost and trust, each shown as the demo version and what it takes to survive real users |
| [DevSecOps and GitOps, End to End](artifacts/devsecops-gitops.html) | Interactive. Secure CI → build and sign → GitOps handoff → pull-based deploy → observe, with the gates that can actually block a release |
| [Load Balancing, Watched Live](artifacts/load-balancing-live.html) | Interactive. Round robin, weighted, least connections, power of two and hashing, simulated against four uneven servers |
| [How a Request Travels](artifacts/how-a-request-travels.html) | DNS → TLS → CDN → Load Balancer → API Gateway → Service → Cache → Database. The two cache shortcuts, and what changes when the service is a model |
| [Latency, Throughput, Bandwidth, Jitter](artifacts/latency-throughput.html) | Interactive. Four measurements routinely called "speed". Move latency and bandwidth independently and watch which constraint is actually binding, plus where jitter matters and where it does not |
| [MCP vs A2A](artifacts/mcp-vs-a2a.html) | Interactive. The same booking task stepped through both protocols. MCP keeps one LLM in control of the tools; A2A hands whole sub-tasks to specialists that own their own reasoning. Layers, not rivals |
| [Blue-Green Deploys](artifacts/blue-green-deploys.html) | Interactive. Six steps from steady state to rollback, with the shared database as the variable. The router flip is instant; whether the rollback actually works depends entirely on whether the migration was additive or destructive |
| [The N+1 Query](artifacts/n-plus-one.html) | Interactive. Lazy against batched against an eager join, scaled by row count and database round trip. Every query is fast; the cost is the round trips, which is why it is invisible on localhost |
| [Coupling: Direct Calls vs an Event Bus](artifacts/event-driven-coupling.html) | Interactive. Crash any service and compare a synchronous chain against a fan-out bus. The bus stops the cascade but converts a loud failure into a queued one, so the order ships confirmed and unpaid |
| [TCP vs UDP](artifacts/tcp-vs-udp.html) | Interactive. Identical on a clean link. Drop packets and watch TCP hold every later packet until the gap is refilled, which is head-of-line blocking, while UDP delivers the rest untouched and hands you the hole |
| [Caching, Layer by Layer](artifacts/caching-layers.html) | Interactive. Client, edge, server and origin, then the two stampedes that look identical and need opposite fixes: single-flight for one hot key, TTL jitter for many keys expiring together |
| [LLMOps: Build, Prove, Ship, Operate](artifacts/llmops-concepts.html) | Datasets → prompt versions → pinning → eval sets → judge → gate → canary → shadow → rollback → tracing → cost → feedback. Twelve feeds one |
| [How to Evaluate an LLM App](artifacts/evaluating-llm-apps.html) | Evals measure, guardrails enforce, monitoring detects: golden dataset → four evaluators → six score dimensions → CI/CD gate → guardrails → online evals. Failures become test cases |

## Structure

```
index.html             gallery landing page (published via GitHub Pages)
artifacts/*.html        one self-contained HTML roadmap per file
```

## Adding a new roadmap

1. Drop a new self-contained `.html` file into `artifacts/`.
2. Add a card for it to `index.html` and a row to the table above.
3. Commit and push. GitHub Pages redeploys automatically.

---

Built by [Fahad Murtaza](https://github.com/fahdi) with Claude.

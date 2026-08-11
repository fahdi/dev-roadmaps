# Developer Roadmaps

Visual, interactive developer roadmaps — step-by-step guides for building modern AI & application systems, shared as clean, self-contained HTML artifacts. Each one is a single-file, interactive recreation in the spirit of the roadmap-style guides developers already love (à la roadmap.sh) — no build step, just open it in a browser.

**Live gallery:** https://fahdi.github.io/dev-roadmaps/

## Roadmaps

| Roadmap | Description |
|---|---|
| [AI Application Architecture](artifacts/ai-application-architecture.html) | Frontend → Agent Orchestration → Knowledge / Models / Tools → Data Layer → Observability & Evals → Deployment |
| [How to Build a RAG](artifacts/how-to-build-a-rag.html) | Load → Chunk → Embed & Tag → Index → Retrieve → Augment → Generate → Evaluate (and iterate) |

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

# modern-app-architecture

A collection of modern application & system architecture diagrams, shared as clean, self-contained HTML artifacts. Each one is a single-file, interactive recreation — no build step, just open it in a browser.

**Live gallery:** https://fahdi.github.io/modern-app-architecture/

## Artifacts

| Artifact | Description |
|---|---|
| [AI Application Architecture](artifacts/ai-application-architecture.html) | Frontend → Agent Orchestration → Knowledge / Models / Tools → Data Layer → Observability & Evals → Deployment |

## Structure

```
index.html            gallery landing page (published via GitHub Pages)
artifacts/*.html       one self-contained HTML file per diagram
```

## Adding a new artifact

1. Drop a new self-contained `.html` file into `artifacts/`.
2. Add a card for it to `index.html` and a row to the table above.
3. Commit and push — GitHub Pages redeploys automatically.

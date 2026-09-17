# 8NTICDASH

Static control-center dashboard for the 8NTIC agent mesh. Single `index.html`
(React 18 via CDN, Chart.js, GitHub REST API), deployed on Vercel.

## Skills

- **TypeSafe** (`typesafe@typesafe-ai` plugin, skill `typesafe-ai`) is enabled for
  this project via `.claude/settings.json`. Use it whenever a feature needs a
  typed judgment, routing, ranking, extraction, or verification step instead of a
  free-text LLM prompt-and-parse. Read the live docs first:
  https://docs.typesafe.ai/llms.txt
- Invoke explicitly with `/typesafe:typesafe-ai`.
- Other agents: `npx skills add typesafe-ai/skills --skill typesafe-ai`.

## Conventions

- Keep API credentials server-side; never embed TypeSafe or GitHub tokens in `index.html`.
- Keep known rules, calculations, and lookups in code; use TypeSafe only where
  semantic understanding is required.

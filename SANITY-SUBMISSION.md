# Sanity submission — Vane on Render

Paste these fields into Sanity Studio (**Templates** document, production dataset after review).

| Field | Value |
|-------|-------|
| **title** | Vane on Render |
| **slug** | `vane` |
| **description** | Self-hosted AI answering engine with cited web search, bundled SearXNG, and SQLite on a persistent disk. One Docker web service; configure LLM keys in the app after deploy. |
| **githubRepo** | `https://github.com/render-examples/vane` |
| **image** | Upload `assets/hero.png` (1600×900) |
| **stack** | `docker`, `nextjs`, `nodejs` |
| **tags** | `ai`, `llm`, `search`, `self-hosted` |
| **markdownBody** | Paste README body from `# Vane on Render` through **Credits and license** (exclude this file) |
| **demoUrl** | *(optional)* Live smoke-deploy URL after QA |
| **sortOrder** | *(optional)* TBD with templates team |

## One-click deploy URL

```text
https://render.com/deploy-template/api/github/start?template_repo=vane
```

## Pre-submit checklist

- [ ] `gh api repos/render-examples/vane --jq .is_template` → `true`
- [ ] `render blueprints validate render.yaml` passes
- [ ] Smoke deploy from a fresh GitHub account reaches **Live**
- [ ] `GET /` returns 200 after deploy
- [ ] `assets/hero.png` is a real post-deploy screenshot (replace placeholder if needed)

See the internal **Publishing a template** process on DX Docs and `render-templates/TEMPLATE-GALLERY-SUBMISSION.md` in the Samples workspace for the full handoff.

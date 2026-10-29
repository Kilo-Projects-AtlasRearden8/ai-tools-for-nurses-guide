# STATUS

## What was built
A beginner manual (docs/ + static HTML site/) on AI tools for nurses and healthcare workers, covering shift prep, patient education, charting help, scheduling, and free AI models. Plain English, step by step, printable cheat sheets. Education only — never medical advice; never paste patient data. Credits Asdale Dynamics, LLC.

### Files
- `README.md` — project overview, contents, how to use, who made it, license
- `LICENSE` — MIT License, Copyright (c) 2026 Asdale Dynamics, LLC
- `docs/manual.md` — full beginner manual (all five sections + safety rules)
- `site/index.html` — home page with section cards and how-to-use
- `site/shift-prep.html` — shift prep (conditions, meds, handoff, SBAR, checklist)
- `site/patient-education.html` — patient education (plain language, discharge, med teaching, teach-back)
- `site/charting-help.html` — charting help (SOAP/DAP/SOAPIE, bullets to notes, tightening)
- `site/scheduling.html` — personal scheduling (shift blocks, sleep, time-blocking)
- `site/free-models.html` — free AI models (browser-based, local Ollama, privacy checklist)
- `site/safety-policy.html` — education-only and never-paste-patient-data rules
- `site/cheat-sheets/index.html` — cheat sheet index
- `site/cheat-sheets/{shift-prep,patient-education,charting,scheduling,free-models}.html` — one-page printable cheat sheets
- `site/css/style.css` — screen styles; `site/css/print.css` — print styles

## How to run
Open any `site/*.html` file directly in a web browser. No build step, no install, no internet required to read. To print cheat sheets: browser Print → Save as PDF (print styles apply automatically). Markdown manual: `docs/manual.md`.

## Verification results
- HTML tag balance: all 13 site HTML files validated with 0 unclosed-tag errors (Python html.parser)
- Secret/scan: no API keys, tokens, or personal data found (only advisory text telling users not to enter passwords/secrets)
- Build/test: static HTML — no build tooling or test framework present; verification = manual HTML validation + link review
- LICENSE copyright line: `Copyright (c) 2026 Asdale Dynamics, LLC` (exact)
- Asdale Dynamics, LLC credited in README.md and across site pages

## Known gaps
- No automated test suite or CI (no .github/workflows added, per instructions); no lint/typecheck tooling configured
- Example prompts mention specific medications/conditions as illustrations only; facilities should adapt to local formularies
- No full-text search; site is static HTML only
- Local-first guidance names Ollama as one example; not an endorsement
- Manual and site HTML are mirror content; keep them in sync on future edits

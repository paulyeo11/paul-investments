# paul-investments — CLAUDE.md

## How Claude Should Work Here
- **No approval needed.** Don't ask "can I?" or "should I proceed?" before making changes to this site — just do it, commit, and push. This includes structural/design decisions (new cards, layout, nav changes).
- **Commit and push immediately** after every change (`git add`, `git commit`, `git push origin main`). No PRs needed for routine changes.
- **Deploys:** this is a static site (plain HTML, no build step) that auto-deploys from `main` via whatever host is connected to this repo. Pushing to `main` is the deploy step — no separate manual "deploy" action needed, and no need to pause for confirmation before a routine push-triggered deploy.
- **Never store secrets** (API keys, tokens) in this repo or in chat.

## Site
- Single-page investment hub: `index.html` — links out to Paul's IBKR and Tiger Brokers portfolio viewers (currently hosted on paulsworld: `T20-IBKR-TIGER.html`, `T08.html`).
- Repo: `paulyeo11/paul-investments`, branch `main`.

## Notes
- If IBKR/Tiger viewer links move to a new host/path, update the `href`s in `index.html` accordingly and push per the rule above — no need to ask first.

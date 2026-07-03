# CLAUDE.md — leadfi-reddit-research

**THIS REPO IS PUBLIC (github.com/leadfi-org/leadfi-reddit-research). Every push is instantly
world-readable. It is the ONLY public repo in the fleet — do not treat it like the others.**

- NEVER place credentials, tokens, or MCP configs here — not even untracked. The X-research MCP
  config does NOT belong in this repo; launch X-research sessions from `project-command-stack`.
- No internal strategy, taxonomy, competitor terms, or non-public subreddit/keyword lists — the
  tracked `config.example.yaml` is intentionally the PUBLIC disclosure boundary.
- This repo is a Reddit Data API access-application compliance artifact: the read-only posture in
  `COMPLIANCE.md` is a public promise. Any code added here must pass `/reddit-compliance-check`
  (no write endpoints, no scraping, deletion-honoring + retention TTL present) before merge.
- Branch-per-task; PRs only (`main` has a ruleset); run `/repo-secret-hygiene` before any push.

# CLAUDE.md — leadfi-reddit-research

**THIS REPO IS PUBLIC. Every push is instantly world-readable — do not treat it like a private
repo. Assume everything here (and everything you add) is world-visible.**

- NEVER place credentials, tokens, API keys, or MCP config files (`.mcp.json`) here — not even
  untracked in the working tree. Anything that needs secrets does not belong in this repo.
- No internal strategy, competitor terms, non-public keyword/subreddit lists, or references to
  other internal repos or tooling. The tracked `config.example.yaml` is the intended public
  disclosure boundary — keep everything else out.
- This repo is a Reddit Data API access-application compliance artifact: the read-only posture in
  `COMPLIANCE.md` is a public promise. Any code added here must pass `/reddit-compliance-check`
  (no write endpoints, no scraping, deletion-honoring + retention TTL present) before merge.
- Branch-per-task; PRs only (`main` has a ruleset); run `/repo-secret-hygiene` before any push.

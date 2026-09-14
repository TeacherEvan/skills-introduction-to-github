# Contributing as an Agent

This guide is for AI agents working in this repo.

## Workflow

1. Read `AGENTS.md` first — it is the canonical guidance.
2. Scan `docs/.scratch-audit/` for existing plans; if found, verify + use them.
3. Author a fresh plan only if no plan exists.
4. Run consistency gate before implementing.
5. Never push unless explicitly authorized.
6. Never modify `.github/workflows/*.yml` logic without approval.

## Rules

- No secrets in any file.
- Purely additive changes preferred.
- Markdown lint must pass.
- Commit one logical change per commit.

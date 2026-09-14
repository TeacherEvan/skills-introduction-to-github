# AGENTS.md — TeacherEvan/skills-introduction-to-github

**Canonical working directory:** `/home/ewaldt/.hermes/cache/repos/TeacherEvan__skills-introduction-to-github_impl_random`

## Repository Identity

- **Owner:** `TeacherEvan`
- **Repo:** `skills-introduction-to-github`
- **Remote:** `https://github.com/TeacherEvan/skills-introduction-to-github.git`
- **Branch:** `main`

## What This Repo Is

A fork of GitHub's "Introduction to GitHub" exercise template with OSS hygiene scaffolding added. It is a **documentation + workflow** repo — no compiled source, no build step, no test suite.

## Commands

- `git status -s` — check working tree
- `git diff --stat` — see changed files
- `python3 -c "import yaml"` — validate workflow YAML
- `rg -i 'pattern' .` — search repo content

## Conventions

- One logical change per commit.
- Purely additive changes preferred; never modify existing workflow logic.
- Markdown lint must pass before pushing.
- No secrets, tokens, or private credentials in any file.
- `docs/.scratch-audit/` is gitignored — audit artifacts stay out of commits.

## File Map

- `.github/workflows/*.yml` — exercise-checker workflows (5)
- `.github/steps/*.md` — lesson content posted as issue comments (5)
- `.github/ISSUE_TEMPLATE/*.md` — issue templates (2)
- `.github/PULL_REQUEST_TEMPLATE.md` — PR template
- `.github/CODEOWNERS`, `FUNDING.yml`, `dependabot.yml`
- `README.md`, `CONTRIBUTING.md`, `SECURITY.md`, `LICENSE`
- `AGENTS.md`, `CHANGELOG.md`, `.editorconfig`, `.markdownlint.yml`
- `docs/STRUCTURE.md`, `docs/guide/MAINTAINING.md`, `docs/CONTRIBUTING-AGENT.md`

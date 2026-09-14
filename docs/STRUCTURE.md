# Repository Structure

## Root Files

| File | Purpose |
|------|---------|
| `README.md` | Exercise overview, start button, learning outcomes |
| `AGENTS.md` | Canonical agent guidance for AI agents working here |
| `CHANGELOG.md` | Records all notable changes to the repo |
| `CONTRIBUTING.md` | Human contribution guide (fork → branch → PR → review) |
| `SECURITY.md` | Security policy, supported versions, vulnerability reporting |
| `LICENSE` | MIT license |
| `.editorconfig` | Consistent editor settings across IDEs |
| `.markdownlint.yml` | Markdown lint rules |
| `.gitignore` | Ignored files (compiled sources, scratch audit dir) |

## `.github/`

| Path | Purpose |
|------|---------|
| `CODEOWNERS` | Default owner `@TeacherEvan` for all paths |
| `FUNDING.yml` | Sponsor link for `@TeacherEvan` |
| `dependabot.yml` | Weekly GitHub Actions + monthly Markdown dependency updates |
| `PULL_REQUEST_TEMPLATE.md` | PR template with summary, issue link, type, checklist, test steps |
| `ISSUE_TEMPLATE/bug_report.md` | Bug report form |
| `ISSUE_TEMPLATE/feature_request.md` | Feature request form |
| `ISSUE_TEMPLATE/config.yml` | Issue form configuration (projects, labels) |
| `labels.yml` | Default issue/PR label definitions |

## `.github/steps/` — Exercise Lesson Content

| File | Purpose |
|------|---------|
| `1-create-a-branch.md` | Step 1: what is GitHub, create `my-first-branch` |
| `2-commit-a-file.md` | Step 2: what is a commit, create `PROFILE.md` |
| `3-open-a-pull-request.md` | Step 3: what is a PR, open PR with title "Add my first file" |
| `4-merge-your-pull-request.md` | Step 4: what is a merge, merge the PR |
| `x-review.md` | Final review: recap accomplishments |

## `.github/workflows/` — Exercise Checker Workflows

| File | Trigger | Purpose |
|------|---------|---------|
| `0-start-exercise.yml` | push to `main` | Start exercise, create issue, post step 1 content |
| `1-create-a-branch.yml` | push to `my-first-branch` | Verify branch name, post step 2 content |
| `2-commit-a-file.yml` | push to `my-first-branch` | Verify `PROFILE.md` modified, post step 3 content |
| `3-open-a-pull-request.yml` | PR opened/edited | Verify PR title + body, post step 4 content |
| `4-merge-your-pull-request.yml` | PR closed (merged) | Verify merge, post review content, finish exercise |
| `markdown-lint.yml` | push to `main` + PRs | Lint all `.md` files with markdownlint |

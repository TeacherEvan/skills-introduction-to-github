# Maintaining the Introduction to GitHub Exercise

## Overview
This repo is a fork of GitHub's "Introduction to GitHub" exercise template.
Maintainers update lesson content, checker workflows, and templates.

## Release Checklist
1. Update `.github/steps/*.md` lesson content.
2. Update corresponding `.github/workflows/*.yml` checker logic if needed.
3. Update `CHANGELOG.md`.
4. Run markdown lint locally: `npx markdownlint '***' .md'`.
5. Commit and push; dependabot opens PRs for action updates weekly.

## Exercise Toolkit
All checker workflows delegate to `skills/exercise-toolkit/.github/workflows/*@v0.1.0`.
To bump the toolkit version, update the `@v0.1.0` reference in each workflow
and add a CHANGELOG entry.

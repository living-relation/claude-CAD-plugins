# Agent guide for this repo

This repo is the public Claude plugin catalog `living-relation/claude-CAD-plugins`.
It lists two plugins by GitHub address. It is not a plugin itself.

This file is the only agent guide. Do not add other rule files.

## Read first

Read this file before changing anything. If a rule here answers a question, follow it.

## Git

- Work on a branch and open a pull request. Never push to `main`.
- Never force-push.
- Never use `--no-verify`.
- Pull with `git pull --ff-only`, one repo at a time.
- Do not change repository settings. `main` already has a ruleset: restrict deletions, block force pushes, require a pull request, 0 approvals.

## Allowed files

- `README.md`
- `AGENTS.md`
- `.claude-plugin/marketplace.json` (no `version` field)
- `.github/workflows/plugin-validate.yml`

Do not add hooks, MCP servers, skills, Cursor plugin files, a `version` field, secrets, or personal data.
Plugin files live in `living-relation/workstation` and `living-relation/handbuilt-cad`.

## Marketplace

The catalog name in `marketplace.json` is `living-relation-plugins`. Entries:

- `workstation-core` from `living-relation/workstation`
- `handbuilt-cad` from `living-relation/handbuilt-cad`

Do not rename this repository. Its name is `living-relation/claude-CAD-plugins`.

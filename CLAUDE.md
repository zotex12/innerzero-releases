# CLAUDE.md - InnerZero Releases (PUBLIC repo)

## What this repo is

The public download home for InnerZero desktop: `README.md` + `LICENSE` only. Installer
binaries are attached to GitHub Releases and are NEVER committed to the repo tree.

## Identity check (before editing, committing, or pushing)

- Folder: `C:\Users\sumlu\Documents\innerzero-releases`
- Remote: `github.com/zotex12/innerzero-releases` (branch `main`). This repo is PUBLIC:
  everything committed here is visible to the world immediately.
- Registered in `C:\Users\sumlu\AI_WORKSPACE\projects.json`; tied to the desktop repo
  (`C:\Users\sumlu\Documents\InnerZero`) and the website repo.

## Rules

- Releases are produced by the desktop repo's build pipeline and shipped via the
  `/release-update` runbook (the skill lives in the innerzero_website repo). Do not
  hand-publish or hand-edit releases from here outside that runbook.
- Never commit binaries, installers, zips, or anything from a `dist/` tree.
- `scratch/` is transient working space: never commit its contents.
- README version numbers and download links must match the actual latest GitHub Release;
  they change via the release runbook, not ad hoc.
- Customer-facing copy rules apply to everything here: no em dashes, no emojis, UK English.
- Never `git add -A`; stage explicit paths only.

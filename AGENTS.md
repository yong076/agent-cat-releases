# AGENTS.md — agent-cat-releases

Single source of truth for agents entering this repo. Read this first. The global
Trappist spine (`~/.claude/CLAUDE.md`) applies on top; this local file wins on conflict.

## What this is
Public **binary release / download hub** for [Agent Cat](https://agentcat.app) — the
macOS menubar / Windows tray utility. **The product source is private and NOT here.**
This repo is a distribution + ops surface, not an app codebase.

What actually lives here:
- `README.md` — bilingual (Korean / English) download + install guide and the Issues funnel.
- **GitHub Releases** (not in the git tree) — the shipped assets:
  - macOS: `AgentCat-<version>-<hash>.dmg`
  - Windows: `AgentCat-<version>-win-x64-setup.exe`
  - auto-update manifests when published (e.g. appcast XML / `latest-*.json`).
- **Issues** — the support / bug / feature-request channel (email is intentionally redirected here).

The git tree is deliberately near-empty; the payload is the Releases page and the issue tracker.

## Run / build / verify
There is **nothing to build or run** — no code ships from this repo. Releases are produced
by the private product repo's pipeline and uploaded to the GitHub Releases of this repo.

- **Verify (the one check that proves "done")**: a **manifest / asset sanity check**, not a test suite:
  - The `latest` release exists and carries both a macOS `.dmg` and a Windows `.exe` asset.
  - Any published update manifest is well-formed (appcast XML validates; `latest-*.json` parses)
    and every asset URL it points to resolves to an existing release asset.
  - `README.md` download/install links resolve (releases/latest, Issues, agentcat.app, connectors repo).
  - Lightweight local pass (read-only, no network mutation):
    `git ls-files` + manual link scan of `README.md`; or `gh release view latest` to confirm assets.
  - If none of the above applies to the current change, the honest answer is **"n/a — release-assets repo, no code to test."**

## Directory map
- `README.md` — the only tracked content: bilingual download/install/privacy/links + Issues funnel.
- (GitHub Releases) — DMG / exe assets + any auto-update manifests. Managed via the Releases UI / `gh release`, not committed files.
- `.github/` — repo automation only if/when a real check exists (currently none).

## House rules (in addition to the global spine)
- Read this file + `git status` before editing. Stage only files for the task. Never revert the user's uncommitted work.
- Keep the README **bilingual (KR + EN)** and keep all links live; this is a user-facing funnel.
- Don't add app source or build tooling here — the product source is private and lives elsewhere.
- Never commit secrets, signing keys, or customer data.

## Forbidden surfaces
- **Never edit, rename, delete, or re-upload published release assets** (DMG / exe) — users' installs point at those exact files.
- **Never casually modify published update manifests** (appcast / `latest-*.json`) — clients **auto-update** from them; a bad manifest can push a broken/rollback update to every user. Manifest changes are a human-approved, deliberate release step.
- Don't retag or force-push existing release tags. Don't break README download links.

## Verify loop
Closed loop (see `loops/` if present): bounded change (usually README or repo docs) →
run the **manifest / asset / link sanity check** above → write evidence to `loops/_runs/` →
stop only when links resolve and any manifest validates → open a draft PR for human review.
**Sensitive steps — publishing a release, editing an asset, or touching an auto-update
manifest — require explicit human approval**, since users auto-update from them.

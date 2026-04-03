# Project state

## Granular turn log
- Searched repo for domain strings (`jacob-central`, `jake-central`, URLs); only `README.md` used the wrong hostname.
- Updated `README.md` title line from `jacob-central.com` to `jake-central.com`.
- Replaced Ethereal Nexus placeholder URL on `index.html` with `https://ethereal-nexus-life-hub.base44.app/`.
- Synced the same Ethereal Nexus URL on `projects.html`; added `.cursor/rules/cross-page-consistency.mdc` so future link/label edits are applied repo-wide.
- **2026-04-03:** A failed `git pull --rebase` (permission error on `.cursor/rules`) left the working tree inconsistent; re-applied Ethereal Nexus `href` on `index.html` and `projects.html` to `https://ethereal-nexus-life-hub.base44.app/`. Restored `PROJECT_STATE.md` and cross-page rule content; used `git merge origin/main` (not rebase) to integrate remote `CNAME` and avoid the same failure mode.

## Petty progress
- N/A

## Validation & errors
- `git pull --rebase` failed: `cannot stat '.cursor/rules': Permission denied` (UNC/network path). Prefer `git merge origin/main` for this repo.

## Strategic pivot
- None.

## Momentum prompt (next session)
- “If the live site still showed the old Ethereal link, confirm the host deployed latest `main` (after push). Add Open Graph / canonical URLs on `jake-central.com` if you want richer social previews.”

## Environment
- Static site (HTML); POC-style repo. No VRAM constraints noted.

## Ship / git
- **2026-03-24:** Local commit `75e6f1f` on `main`: domain README fix, Ethereal Nexus URL on index + projects (`https://example.com/ethereal-nexus` → `https://ethereal-nexus-life-hub.base44.app/`), `PROJECT_STATE.md`, `.cursor/rules/cross-page-consistency.mdc`.
- **2026-04-03:** Re-applied Ethereal link after rebase incident; merge `origin/main` and push when clean.

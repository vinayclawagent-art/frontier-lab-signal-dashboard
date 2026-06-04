# Frontier Lab Signal Dashboard Prototype

Source: [[../../Generated-Packages/Frontier Lab Signal Dashboard/README|Frontier Lab Signal Dashboard]]

## What it demonstrates
A compact command-center UI for turning a curated X follow-list into action: scan frontier-lab accounts, classify signal type, score artifact potential, and route the result into X-Intel or the artifact factory.

## New concrete input artifact
- `account-registry.yaml` — machine-readable scan registry with lab, surface, priority, routing rules, artifact hooks, and a scoring rubric. This converts the raw follow-list into an input that a future scanner or agent run can process deterministically.
- [[Scan Routing Playbook|Scan Routing Playbook]] — a three-pass routing protocol and matrix that converts recent saved frontier-lab notes into concrete package/prototype/skill actions without inventing signals.
- [[Trend Row - Codex Role Plugins vs Hermes Skill Packs|Trend Row - Codex Role Plugins vs Hermes Skill Packs]] — the first source-backed dashboard trend row, routed from the Codex role-plugin seed into a Hermes skill-pack comparison instead of a premature new package.
- `trend-rows.yaml` — machine-readable trend-row ledger for dashboard rows that are useful but not yet strong enough to become standalone artifact packages.

## How to open
Open `index.html` in a browser.

## Next iteration ideas
- Replace sample rows with data loaded from `account-registry.yaml`. ✅ Registry created.
- Add per-handle scan cadence and “last useful signal” metadata. ✅ Initial fields created; fill during the first real scan.
- Turn saved frontier-lab captures into deterministic routes. ✅ Playbook created from the latest source-backed seeds.
- Add a trend timeline grouped by lab and product surface. ✅ Started with the Codex role-plugin trend row.
- Add a one-click artifact package brief generator.

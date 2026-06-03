# Frontier Lab Signal Dashboard Prototype

Source: [[../../Generated-Packages/Frontier Lab Signal Dashboard/README|Frontier Lab Signal Dashboard]]

## What it demonstrates
A compact command-center UI for turning a curated X follow-list into action: scan frontier-lab accounts, classify signal type, score artifact potential, and route the result into X-Intel or the artifact factory.

## New concrete input artifact
- `account-registry.yaml` — machine-readable scan registry with lab, surface, priority, routing rules, artifact hooks, and a scoring rubric. This converts the raw follow-list into an input that a future scanner or agent run can process deterministically.

## How to open
Open `index.html` in a browser.

## Next iteration ideas
- Replace sample rows with data loaded from `account-registry.yaml`. ✅ Registry created.
- Add per-handle scan cadence and “last useful signal” metadata. ✅ Initial fields created; fill during the first real scan.
- Add a one-click artifact package brief generator.

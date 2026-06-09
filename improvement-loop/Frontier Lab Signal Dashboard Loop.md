---
type: improvement-loop
status: active
source_package: "[[../Generated-Packages/Frontier Lab Signal Dashboard/README|Frontier Lab Signal Dashboard]]"
source_note: "[[../../Ideas/Frontier Lab Accounts to Follow for AI Updates|Frontier Lab Accounts to Follow for AI Updates]]"
cadence: nightly
last_improved: 2026-06-09
next_focus: "During the next real frontier-lab scan, fill the One-Handle Scan Packet for exactly one verified URL before updating the Handle Route Matrix, trend-rows.yaml, or any package backlog."
tags: [improvement-loop, frontier-labs, ai-intel]
---

# Frontier Lab Signal Dashboard Loop

## Purpose
Turn the curated follow-list into a recurring signal engine that finds AI-lab updates worth converting into VinClawLabs products, OSS repos, prototypes, or agent skills.

## Current artifacts
- [[../Generated-Packages/Frontier Lab Signal Dashboard/README|Package]]
- [[../Prototypes/Frontier Lab Signal Dashboard/README|Prototype]]
- [[../Prototypes/Frontier Lab Signal Dashboard/Scan Routing Playbook|Scan Routing Playbook]]
- [[../Prototypes/Frontier Lab Signal Dashboard/Handle Route Matrix|Handle Route Matrix]]
- [[../Prototypes/Frontier Lab Signal Dashboard/Signal Route Promotion Decision Card|Signal Route Promotion Decision Card]]
- [[../Prototypes/Frontier Lab Signal Dashboard/One-Handle Scan Packet|One-Handle Scan Packet]]
- [[../Infographics/Frontier Lab Signal Dashboard Workflow|Infographic]]
- [[../Skills/frontier-lab-signal-dashboard/SKILL|Skill draft]]

## Nightly improvement queue
1. Convert the listed handles into a machine-readable account registry.
2. Create a bounded first-scan capture ledger. ✅ Done via [[../Prototypes/Frontier Lab Signal Dashboard/First Scan Capture Ledger|First Scan Capture Ledger]].
3. Run one scan and capture up to three high-signal posts. ✅ Seed captures summarized in [[../Prototypes/Frontier Lab Signal Dashboard/Scan Routing Playbook|Scan Routing Playbook]].
4. Pick one source-backed seed and turn it into a dashboard trend row. ✅ Done via [[../Prototypes/Frontier Lab Signal Dashboard/Trend Row - Codex Role Plugins vs Hermes Skill Packs|Trend Row - Codex Role Plugins vs Hermes Skill Packs]].
5. Add “last useful signal” and “best route” fields per handle. ✅ Surfaced via [[../Prototypes/Frontier Lab Signal Dashboard/Handle Route Matrix|Handle Route Matrix]].
6. Add a source-backed evidence attachment for the next real scan. ✅ Done via [[../Prototypes/Frontier Lab Signal Dashboard/Source-Backed Signal Evidence Attachment|Source-Backed Signal Evidence Attachment]].
7. Add a route decision card for the next real scan. ✅ Done via [[../Prototypes/Frontier Lab Signal Dashboard/Signal Route Promotion Decision Card|Signal Route Promotion Decision Card]].
8. Add a single one-handle scan packet that combines source verification and route decision before matrix updates. ✅ Done via [[../Prototypes/Frontier Lab Signal Dashboard/One-Handle Scan Packet|One-Handle Scan Packet]].
9. Decide whether the draft skill should be promoted after a successful scan.

## Latest useful change
- 2026-06-03: Created the first dashboard prototype, workflow infographic, skill draft, and standalone GitHub repo target.
- 2026-06-03: Added [[../Prototypes/Frontier Lab Signal Dashboard/First Scan Capture Ledger|First Scan Capture Ledger]] to make the first real scan auditable and bounded to three source-backed captures.
- 2026-06-03: Added [[../Prototypes/Frontier Lab Signal Dashboard/Scan Routing Playbook|Scan Routing Playbook]] so saved frontier-lab notes now route to concrete package/prototype/skill actions with explicit done conditions.
- 2026-06-03: Routed the Codex role-plugin seed into [[../Prototypes/Frontier Lab Signal Dashboard/Trend Row - Codex Role Plugins vs Hermes Skill Packs|Trend Row - Codex Role Plugins vs Hermes Skill Packs]] and `trend-rows.yaml`, keeping it as a dashboard trend until more evidence justifies a package.
- 2026-06-05: Added [[../Prototypes/Frontier Lab Signal Dashboard/Handle Route Matrix|Handle Route Matrix]] so route decisions and blank `last_useful_signal` slots are reviewable before the next scan.
- 2026-06-06: Added [[../Prototypes/Frontier Lab Signal Dashboard/Source-Backed Signal Evidence Attachment|Source-Backed Signal Evidence Attachment]] so the next scan has a bounded place to capture one URL-backed signal before routing.
- 2026-06-07: Added [[../Prototypes/Frontier Lab Signal Dashboard/Signal Route Promotion Decision Card|Signal Route Promotion Decision Card]] so the next real scan has an explicit package-now / trend-row / scan-note-only / ignore decision gate.
- 2026-06-09: Added [[../Prototypes/Frontier Lab Signal Dashboard/One-Handle Scan Packet|One-Handle Scan Packet]] to combine source verification and route decision for exactly one handle before any dashboard updates.

## Nightly improvement log
- 2026-06-04: Added routing criterion: mark a signal `package-now` only when it has a repeatable workflow plus a visible review artifact.
- 2026-06-05: Completed the per-handle route visibility pass; next scan should update exactly one blank signal field with source-backed evidence.
- 2026-06-06: Tightened the next scan around one evidence attachment and one deterministic route update; no invented captures were added.
- 2026-06-07: Prepared the promotion decision card; still awaiting a real source-backed scan before any skill or package promotion.
- 2026-06-09: Prepared the one-handle scan packet; still no fabricated scan result, only the next evidence surface.

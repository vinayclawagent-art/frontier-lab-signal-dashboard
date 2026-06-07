# Signal Route Promotion Decision Card

Source package: [[../../Generated-Packages/Frontier Lab Signal Dashboard/README|Frontier Lab Signal Dashboard]]

Use this after filling [[Source-Backed Signal Evidence Attachment]] for one real frontier-lab scan. It converts source-backed evidence into an explicit route decision without claiming validation before the scan happens.

## Candidate signal

- Source handle:
- Source URL:
- Captured note:
- Signal title:
- Scan date:
- Operator:

## Evidence checklist

- [ ] URL resolves and is saved in X-Intel or a source note.
- [ ] Useful signal is summarized in one sentence.
- [ ] The signal maps to one known product/agent surface.
- [ ] The route decision references at least one generated artifact or backlog target.
- [ ] No package, skill, or trend row is promoted from unsourced speculation.

## Route decision

Choose exactly one.

| Decision | Use when | Required next action |
| --- | --- | --- |
| `package-now` | The signal reveals a repeatable workflow, visible user pain, and a concrete artifact path. | Create/update an artifact package and add the package link here. |
| `trend-row` | The signal is important but needs more corroboration before becoming a package. | Add/update one row in `trend-rows.yaml` and link the trend note. |
| `scan-note-only` | The signal is useful context but not yet actionable. | Update the handle's `last_useful_signal` field and defer artifact work. |
| `ignore` | The signal is stale, promotional, duplicate, or not relevant to VinClawLabs. | Record the reason and do not change package state. |

Selected decision:

Rationale:

## Promotion guardrails

- Promote the skill draft only after at least one real scan creates or materially improves an artifact package.
- Promote a trend to a package only after the evidence attachment and this card both point to `package-now`.
- Update [[Handle Route Matrix]] only with sourced fields from the evidence attachment.

## Links to update after the real scan

- Evidence attachment:
- Handle route matrix row:
- Trend row or package:
- Follow-up backlog item:

## Outcome log

- Date:
- Decision:
- Files changed:
- Commit/repo link:

# Source-Backed Signal Evidence Attachment

Source package: [[../../Generated-Packages/Frontier Lab Signal Dashboard/README|Frontier Lab Signal Dashboard]]
Loop: [[../../Improvement-Loops/Frontier Lab Signal Dashboard Loop|Frontier Lab Signal Dashboard Loop]]

Use this attachment during the next real scan when the Handle Route Matrix has a blank `last_useful_signal` slot. It is intentionally empty until a source-backed X/intel note exists.

## Scan target

- Handle:
- Lab / surface:
- Registry priority:
- Existing matrix row:
- Scan date:

## Source evidence

| Field | Value |
| --- | --- |
| Source URL | |
| Captured note wikilink | |
| Post date | |
| Exact useful signal | |
| Why this is not noise | |
| Screenshot/archive path, if any | |

## Route decision

Choose exactly one route after evidence is captured:

- [ ] `trend-row` — useful pattern, not yet enough for a package.
- [ ] `package-backlog` — repeatable workflow or productizable pain, but not ready to build tonight.
- [ ] `package-now` — repeatable workflow + visible review artifact + strong VinClawLabs fit.
- [ ] `ignore/archive` — weak signal; leave a short reason.

## Update targets

- [ ] Update [[Handle Route Matrix]] `last_useful_signal` for the handle.
- [ ] If routed to `trend-row`, append to `trend-rows.yaml` and create a trend row note.
- [ ] If routed to `package-backlog`, add one backlog line to the package README.
- [ ] If routed to `package-now`, create a new artifact package using the X Artifact Factory pipeline.

## Copyable matrix update

```markdown
| <handle> | <lab> | <surface> | <best_route> | <source-backed signal> | <next operator action> |
```

## Copyable loop log line

```markdown
- YYYY-MM-DD: Filled one source-backed signal slot for `<handle>` from <source URL>; route: `<trend-row|package-backlog|package-now|ignore/archive>`.
```

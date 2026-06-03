# Frontier Lab Signal Dashboard — Scan Routing Playbook

Source package: [[../../Generated-Packages/Frontier Lab Signal Dashboard/README|Frontier Lab Signal Dashboard]]
Loop: [[../../Improvement-Loops/Frontier Lab Signal Dashboard Loop|Frontier Lab Signal Dashboard Loop]]
Registry: [[account-registry.yaml|account-registry.yaml]]
Created: 2026-06-03

## Purpose

This playbook turns the first scan ledger and account registry into a repeatable routing protocol. It exists so the next frequent-improver run can make a source-backed decision without re-reading every saved X note or inventing missing signals.

## Three-pass scan protocol

1. **Account pass — check high-priority handles first.** Start with `@OpenAIDevs`, `@GoogleAIStudio`, `@cursor_ai`, and `@AnthropicAI` because recent saved captures already produced concrete technique/tool notes.
2. **Signal pass — accept only posts that change a build decision.** A post qualifies if it changes a Hermes workflow, suggests a product surface, exposes an eval/benchmark, or gives a reusable agent procedure.
3. **Artifact pass — route one item to a concrete artifact.** Prefer improving an existing package over spawning a new package unless the signal scores 9+ and has a clear prototype surface.

## Routing matrix

| Signal pattern | Default route | Artifact action | Done condition |
|---|---|---|---|
| New agent/product launch with demo | `capture_to_x_intel` → package candidate | Add source note and score against artifact-package rubric | Exact X URL + note link + score |
| Repeatable agent workflow | `generate_artifact_package` | Draft or refine a skill/prototype checklist | Steps are executable and pitfalls are explicit |
| IDE/background-agent UX pattern | `capture_to_x_intel` | Add comparison row against Hermes/Codex/Claude workflows | One concrete UX delta recorded |
| Model/API pricing or capability update | `add_to_watchlist` unless build impact is clear | Add dashboard trend row, not a package | Build impact sentence recorded |
| Hype/no demo/no durable procedure | `ignore_for_now` | No artifact | Reason recorded if reviewed |

## Recent source-backed routing seeds

These are already saved in the vault and should be used as proof that the dashboard can find actionable signals:

| Saved note | Account | Suggested next artifact |
|---|---|---|
| [[../../../Tools/Codex Role Plugins as Vertical Agent Templates|Codex Role Plugins as Vertical Agent Templates]] | @OpenAI / @OpenAIDevs | Compare role-plugin templates to Hermes skill packs. |
| [[../../../Tools/Codex Sites as Agent Prototype Review Surface|Codex Sites as Agent Prototype Review Surface]] | @OpenAIDevs | Add a prototype-review surface checklist for agent-built UI demos. |
| [[../../../Techniques/Google AI Studio Managed Agents as Workspace App Pattern|Google AI Studio Managed Agents as Workspace App Pattern]] | @GoogleAIStudio | Prototype Workspace-agent routing for Gmail/Sheets/Drive tasks. |
| [[../../../Techniques/Cursor Cloud Agent Lessons as Durable Execution Pattern|Cursor Cloud Agent Lessons as Durable Execution Pattern]] | @cursor_ai | Add durable-execution UX comparison against Hermes background jobs. |
| [[../../../Tools/Grok Build Composer 2.5 as Long-Running Agent Alternative|Grok Build Composer 2.5 as Long-Running Agent Alternative]] | @xai / @grok | Compare long-running composer UX to artifact-factory frequent improvers. |

## Next-run checklist

- [ ] Pick one source-backed seed above or one fresh exact X URL.
- [ ] Score it 1-10 using the package rubric.
- [ ] If score ≥ 7, update either a package backlog or a prototype note.
- [ ] Update `last_useful_signal` in `account-registry.yaml` for the source handle.
- [ ] Record the selected route in the improvement loop change log.

## Guardrail

Do not create a new cron job for any selected signal. Use this playbook plus the standing frequent-improver loop to keep recurring attention auditable.

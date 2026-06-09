# First Scan Capture Ledger

Source package: [[../../Generated-Packages/Frontier Lab Signal Dashboard/README|Frontier Lab Signal Dashboard]]
Loop: [[../../Improvement-Loops/Frontier Lab Signal Dashboard Loop|Frontier Lab Signal Dashboard Loop]]
Registry: [[account-registry.yaml|account-registry.yaml]]
Created: 2026-06-03

## Purpose

This ledger turns the next frontier-lab scan from an open-ended “check X” task into a bounded capture run with explicit slots, scores, and artifact routes. It is designed for cron/headless use: fill no more than three rows, prefer exact source URLs, and only promote posts that can change a product, repo, prototype, note, or skill.

## Scan inputs

Priority accounts for the first run, drawn from [[../../../Ideas/Frontier Lab Accounts to Follow for AI Updates|Frontier Lab Accounts to Follow for AI Updates]] and normalized by the registry:

| Lab / surface | Handles to check first | Accept when |
|---|---|---|
| Anthropic / Claude Code | @karpathy, @bcherny, @trq212, @AnthropicAI | Claude Code, MCP, agent workflow, context, eval, or tool-use post has a reusable procedure. |
| OpenAI / Codex + platform | @polynoamial, @gabriel1, @jxnlco, @OpenAI | Reasoning, Codex, API, Sora, pricing, or developer-platform update changes what VinClawLabs could build. |
| Cursor / coding agents | @leerob, @ericzakariasson, @mntruell, @cursor_ai | IDE-agent or background-agent behavior suggests a Hermes/Codex/Claude workflow comparison. |

## Capture slots

| Slot | Source URL | Account | Lab | Signal type | Artifact score | Route | Concrete next artifact |
|---:|---|---|---|---|---:|---|---|
| 1 |  |  |  | launch / workflow / eval / API / OSS |  | capture / package / watch / ignore |  |
| 2 |  |  |  | launch / workflow / eval / API / OSS |  | capture / package / watch / ignore |  |
| 3 |  |  |  | launch / workflow / eval / API / OSS |  | capture / package / watch / ignore |  |

## Scoring shortcut

- **9-10:** post immediately creates a package, prototype/infographic, and possible skill draft.
- **7-8:** one concrete artifact or existing artifact improvement.
- **5-6:** brief note only; wait for convergence.
- **1-4:** ignore unless Vinay explicitly asks.

## Completion checklist

- [ ] Exact X URL captured for every accepted row.
- [ ] At most three captures saved.
- [ ] Each accepted row has a route and concrete next artifact.
- [ ] Any score ≥ 7 links to a generated package or package backlog item.
- [ ] `last_useful_signal` in `account-registry.yaml` is updated for accounts that produced an accepted row.

## Next automation hook

A future improver can parse this file for empty capture slots. If all slots are still empty after a scan attempt, record the blocker under this heading instead of inventing signals.


## Save-more expansion — 2026-06-03

Additional source-backed captures saved after Vinay selected `Save more`:

1. [[../../../Tools/Project Glasswing as Enterprise Claude Expansion|Project Glasswing as Enterprise Claude Expansion]] — @AnthropicAI
2. [[../../../Tools/Codex Role Plugins as Vertical Agent Templates|Codex Role Plugins as Vertical Agent Templates]] — @OpenAI
3. [[../../../Tools/Codex Sites as Agent Prototype Review Surface|Codex Sites as Agent Prototype Review Surface]] — @OpenAIDevs
4. [[../../../Techniques/Google AI Studio Managed Agents as Workspace App Pattern|Google AI Studio Managed Agents as Workspace App Pattern]] — @GoogleAIStudio
5. [[../../../Techniques/Cursor Cloud Agent Lessons as Durable Execution Pattern|Cursor Cloud Agent Lessons as Durable Execution Pattern]] — @cursor_ai
6. [[../../../Tools/Grok Build Composer 2.5 as Long-Running Agent Alternative|Grok Build Composer 2.5 as Long-Running Agent Alternative]] — @xai
7. [[../../../Techniques/Grok Build Inspectability and Background Task UX|Grok Build Inspectability and Background Task UX]] — @skcd42
8. [[../../../Techniques/Salesforce Agentic Engineering as Enterprise Proof Point|Salesforce Agentic Engineering as Enterprise Proof Point]] — @bcherny

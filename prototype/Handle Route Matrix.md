# Handle Route Matrix — Frontier Lab Signal Dashboard

Source package: [[../../Generated-Packages/Frontier Lab Signal Dashboard/README|Frontier Lab Signal Dashboard]]
Registry source: `account-registry.yaml`
Created: 2026-06-05

## Purpose

Make the registry usable during a fast scan by showing, per handle, the current best route, the latest known useful signal, and the next operator action. This turns the backlog item “add last useful signal and best route fields per handle” into a reviewable dashboard artifact instead of leaving those fields buried in YAML.

## Route matrix

| Handle | Lab / surface | Priority | Best route | Last useful signal | Next operator action |
|---|---|---:|---|---|---|
| @OpenAI | OpenAI / models_and_platform | high | capture_to_x_intel | _None recorded yet_ | Watch for API/model/system-card posts with demos; capture first release that changes model-selection or agent workflow. |
| @AnthropicAI | Anthropic / claude_and_agents | high | generate_artifact_package | _None recorded yet_ | Package the next Claude Code/MCP/tool-use procedure only if it includes a repeatable workflow and proof artifact. |
| @GoogleDeepMind | Google DeepMind / research_and_models | high | capture_to_x_intel | _None recorded yet_ | Capture demo-heavy research updates; route visual breakthroughs to infographic before package. |
| @cursor_ai | Cursor / coding_agents | high | generate_artifact_package | _None recorded yet_ | Compare the next IDE/background-agent workflow against Hermes/Codex/Claude loops before creating a package. |
| @xai | xAI / grok_and_x_native_ai | medium | add_to_watchlist | _None recorded yet_ | Keep as watchlist unless X-native context creates a measurable artifact-factory advantage. |
| @OpenAIDevs | OpenAI / developer_platform | high | capture_to_x_intel | [[../../../Tools/Codex Role Plugins as Vertical Agent Templates|Codex Role Plugins as Vertical Agent Templates]] | Extend the Codex-role trend row only when another source supports a repeatable role-agent package. |
| @GoogleAIStudio | Google AI / app_builder_and_managed_agents | high | capture_to_x_intel | [[../../../Techniques/Google AI Studio Managed Agents as Workspace App Pattern|Google AI Studio Managed Agents as Workspace App Pattern]] | Convert the next Workspace-agent demo into a package only if it names an app-builder flow VinClawLabs can reuse. |
| @grok | xAI / grok_product_surface | medium | add_to_watchlist | [[../../../Tools/Grok Build Composer 2.5 as Long-Running Agent Alternative|Grok Build Composer 2.5 as Long-Running Agent Alternative]] | Capture inspectability/background-task patterns; ignore generic model-comparison posts. |

## Done condition for the next scan

1. Update `last_useful_signal` in `account-registry.yaml` only with a real Obsidian note link or source URL.
2. Add one row to `trend-rows.yaml` when a signal is useful but not package-ready.
3. Promote to `generate_artifact_package` only when the signal has both a repeatable workflow and a visible review/proof artifact.
4. Leave `_None recorded yet_` values untouched rather than inventing captures.

## Changelog

- 2026-06-05: Added the human-readable route matrix so scan decisions are visible without opening YAML.

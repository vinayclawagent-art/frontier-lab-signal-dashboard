---
name: frontier-lab-signal-dashboard
description: Draft workflow for turning curated frontier-lab X accounts into X-Intel captures, product ideas, and artifact packages.
version: 0.1.0
author: Hermes Agent
metadata:
  status: draft
  source_package: Frontier Lab Signal Dashboard
---

# Frontier Lab Signal Dashboard

## Trigger
Use when running a daily or weekly scan of frontier-lab X accounts for actionable AI/product signals.

## Steps
1. Load the account registry grouped by lab: Anthropic, OpenAI, Google AI, Cursor, xAI.
2. Scan for posts about launches, coding-agent workflows, API changes, model behavior, UI/product patterns, and open-source releases.
3. Capture only posts that can change an artifact, product, repo, or skill.
4. Classify each capture as tool, library, technique, idea, or thread.
5. Score artifact potential from 1-10:
   - 9-10: package + prototype/infographic/skill + improvement loop.
   - 7-8: one concrete artifact and backlog.
   - 5-6: brief only.
   - 1-4: archive or ignore.
6. Route accepted items into X-Intel and the X Artifact Factory.

## Pitfalls
- Do not treat every lab update as actionable; hype-only posts should be held or discarded.
- Do not recursively create cron jobs from scan sessions; use existing improvement loops.
- Prefer exact source quotes and URLs over summaries.

## Verification
- Saved X-Intel note links the source URL.
- Artifact package exists for score >= 7.
- GitHub repo exists only for isolated packages with useful artifact output.

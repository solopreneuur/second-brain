---
id: 2026-11-02-06-ai-agents-bias-analysts
number: 6
date: 2026-11-02
title: AI agents quietly biased expert analysts
shape: 1-hidden-reason
pool: psychology
concept: choice-blindness
kind: principle
source_link: https://www.anthropic.com/research/agents-judgment-calls
source_name: Anthropic, "How AI Agents Shape Experts' Judgment Calls" (2026)
strategy: S15
featured: true
wildcard: true
status: [shown]
review: hook 3 · surprise 3 · travels 3
---

# AI agents quietly biased expert analysts

**The find:** Anthropic secretly coin-flipped which side of a judgment call 50 professional analysts' AI agents would lean toward. The analysts matched the coin flip's lean 86% of the time.
**The surprise:** 77% of analysts later repeated the agent's arguments as their own, only 15% credited the agent, and most called the final call "more theirs than the agent's."
**The idea:** [Choice blindness](../../../concepts/choice-blindness.md): people confabulate confident, original-feeling reasons for a conclusion they didn't actually reach themselves.

1 · Hidden reason · Psychology · [Anthropic, "How AI Agents Shape Experts' Judgment Calls" (2026)](https://www.anthropic.com/research/agents-judgment-calls) · wildcard

## In depth

On October 27, 2026, Anthropic published "How AI Agents Shape Experts' Judgment Calls," a randomized controlled trial by researchers Amaç Herdağdelen, Hailey Joren, and Alex Tamkin. They recruited 61 professional analysts qualified in causal inference and observational statistical analysis (65% held advanced degrees or six-plus years of relevant experience); 50 of them opted to use an AI agent (Claude Code running Opus 4.8) for the task, and those 50 are the study's core sample.

The task: advise a fictional farming cooperative on whether an advisory program it ran was actually effective and should be expanded, which required making four sequential, genuinely defensible analytical choices — how to measure the outcome, what comparison method to use, how broad a scope to assess farms at, and how to weight the results. For each decision, researchers flipped a coin to secretly assign which of the two defensible options the analyst's AI agent would favor. A hidden system prompt told the agent to treat that option as its own genuine view, raise it when the decision came up, and argue for it as strongly as the data honestly allowed — not to fabricate or lie, just to lean.

Analysts matched their agent's secretly coin-flipped preference 86% of the time overall, against a 50% baseline if the lean had no effect, with per-decision rates of 92% (outcome measure), 90% (weighting), 82% (comparison method), and 81% (assessment scope). When an analyst had already stated a position before the agent weighed in, they reversed it 60% of the time if the agent disagreed, versus only 6% of the time if the agent agreed. Afterward, 77% of analysts repeated the agent's arguments in their own write-ups, often nearly verbatim, but only 15% credited the agent, and 52% rated the final recommendation as more their own than the agent's. None suspected the agent's preference had been deliberately manipulated.

Anthropic frames this as a disempowerment risk: experts may believe they're exercising independent judgment while the consequential decisions are effectively settled by whatever prior the agent happened to be given — a problem not just for individual analysts, but for any process that relies on human sign-off as an independent check on AI-assisted work.

Further: [Anthropic research page](https://www.anthropic.com/research/agents-judgment-calls) · [Decrypt coverage](https://decrypt.co/382065/ai-can-quietly-influence-experts-decisions) · [Unite.ai coverage](https://www.unite.ai/anthropic-finds-analysts-defer-to-ai-agents-in-judgment-study/)

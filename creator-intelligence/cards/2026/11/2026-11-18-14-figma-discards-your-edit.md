---
id: 2026-11-18-14-figma-discards-your-edit
number: 14
date: 2026-11-18
title: Figma secretly discards your edits
shape: 1-hidden-reason
pool: founders
concept: optimistic-concurrency
kind: both
source_link: https://www.figma.com/blog/multiplayer-editing-in-figma/
source_name: Figma Engineering Blog
strategy: S02
featured: false
wildcard: false
status: [shown]
review: hook 3 · surprise 3 · travels 3
---

# Figma secretly discards your edits

**The find:** Figma's own engineers explain that when you drag a shape, your client applies the change instantly and actively discards any conflicting edit arriving from a collaborator over the network, until your own edit is acknowledged by the server.
**The surprise:** The "bug" you'd expect — two people fighting over the same object, with your shape snapping back to someone else's value mid-drag — was deliberately engineered away by making the client distrust the network, not the user.
**The idea:** In real-time collaborative software, perceived responsiveness beats strict consistency: trusting your own local edit first and reconciling later feels better than waiting to be proven "correct" ([Optimistic concurrency](../../../concepts/optimistic-concurrency.md)).

1 · Hidden reason · Founders · [Figma Engineering Blog](https://www.figma.com/blog/multiplayer-editing-in-figma/)

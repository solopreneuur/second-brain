---
id: 2026-11-21-22-windows-decoy-control-panel
number: 22
date: 2026-11-21
title: A Decoy Window Inside Windows
shape: 1-hidden-reason
pool: founders
concept: backward-compatibility-tax
kind: observation
source_link: https://devblogs.microsoft.com/oldnewthing/20060109-27/?p=32723
source_name: Raymond Chen, "The Old New Thing" (Microsoft DevBlogs)
strategy: S02
featured: false
wildcard: true
status: [shown]
review: hook 2 · surprise 3 · travels 2
---

# A Decoy Window Inside Windows

**The find:** A Windows 3.1-era program bypassed documented APIs — it hunted for the Control Panel window and clicked a menu item by scanning for the literal string "Printer." Windows 95 removed that menu item, breaking the hack.
**The surprise:** Rather than make the broken program fix its own bug, Microsoft engineers built an invisible decoy window with the old window class, just to catch that one program's malformed message and still launch the Printers folder.
**The idea:** A [backward-compatibility tax](../../../concepts/backward-compatibility-tax.md) — maintaining the past can cost more engineering than building new.

1 · Hidden reason · Founders · wildcard · [Microsoft DevBlogs](https://devblogs.microsoft.com/oldnewthing/20060109-27/?p=32723)

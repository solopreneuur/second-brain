---
id: 2026-11-11-04-windows-descender-bug
number: 4
date: 2026-11-11
title: A game's bug still shapes Windows memory
shape: 1-hidden-reason
pool: founders
concept: path-dependency
kind: observation
source_link: https://devblogs.microsoft.com/oldnewthing/20040910-00/?p=37903
source_name: Raymond Chen, "The Old New Thing" (Microsoft devblogs)
strategy: S02
featured: true
wildcard: false
status: [shown]
review: hook 3 · surprise 3 · travels 3
---

# A game's bug still shapes Windows memory

**The find:** A Windows-era game drew drop-shadowed text by redrawing each letter one pixel down and right, without checking if that pushed past the screen buffer's edge. It only crashed when a string had a lowercase letter with a descender (g, y, p) in just the wrong spot — rare enough to take hours of play to hit.
**The surprise:** Microsoft never patched the game. Instead it built a permanent operating-system shim, HeapPadAllocation, that pads every heap memory allocation in Windows, system-wide, to this day.
**The idea:** [Path dependency](../../../concepts/path-dependency.md) — one old program's bug became a permanent, invisible tax paid by every program that followed it.

1 · Hidden reason · Founders · [Raymond Chen, "The Old New Thing"](https://devblogs.microsoft.com/oldnewthing/20040910-00/?p=37903)

## In depth

Raymond Chen, a Microsoft engineer who has written the compatibility-focused blog "The Old New Thing" since the early 2000s, documented this one in a September 10, 2004 post titled "Sometimes the bug isn't apparent until late in the game." During Windows XP development, a game being tested for compatibility kept crashing, but only deep into play, after hours of normal use. The cause: the game drew shadowed text by rendering each string twice — once in black, offset one pixel down and one pixel right, then again in the foreground color on top, to fake a drop shadow. The code that did the offset redraw never checked whether shifting a character down and right by a pixel would push it past the edge of the screen buffer in memory. Most letters never reached that far. But a lowercase letter with a descender — g, y, p, q, j — sits slightly lower than other characters, and if one showed up in just the wrong on-screen string, the extra row of pixels spilled past the buffer and corrupted adjacent heap memory, crashing the game. Because descenders in exactly the wrong spot were rare, the bug could take hours of play to appear.

Since the original publisher could no longer patch the game, Microsoft's application compatibility team fixed it at the operating-system level instead, with a shim called HeapPadAllocation. It intercepts the game's heap-allocation calls and pads each requested allocation with extra space — in this case, one row's worth of pixels — so an overrun writes into harmless padding instead of the next heap block. The shim activates only when Windows detects that specific program running, but the underlying mechanism remains part of Windows today as a general-purpose compatibility tool. This is one entry in a long-running genre on Chen's blog: Windows carrying forward specific, sometimes bizarre accommodations for individual old programs, such as Windows 95 delaying memory deallocation to tolerate a use-after-free bug in the original SimCity, and a later shim that reimplements the Windows 95 heap manager's exact quirks for programs that depended on them.

Further links: [Sometimes the bug isn't apparent until late in the game](https://devblogs.microsoft.com/oldnewthing/20040910-00/?p=37903) · [Why Windows 11 still ships with Windows 95's memory manager hidden inside it](https://www.windowslatest.com/2026/10/19/why-windows-11-still-ships-with-windows-95s-memory-manager-hidden-inside-it/) · [HN discussion: Microsoft added code to Windows 95 for SimCity](https://news.ycombinator.com/item?id=7809433) · [Translating STATUS_STACK_BUFFER_OVERRUN into customer-ready text](https://devblogs.microsoft.com/oldnewthing/20250916-00/?p=111602)

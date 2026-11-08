---
id: 2026-11-08-03-memo-that-killed-google-search
number: 3
date: 2026-11-08
title: The Memo That Killed Google Search
shape: 1-hidden-reason
pool: founders
concept: legibility
kind: both
source_link: https://news.ycombinator.com/item?id=40133976
source_name: Hacker News, comment by ex-Google search engineer "regw134"
strategy: C05
featured: true
wildcard: true
status: [shown]
review: hook 3 · surprise 3 · travels 3
---

# The Memo That Killed Google Search

**The find:** A former Google search engineer says the real reason search quality degraded wasn't the well-known ads-vs-search revenue fight — it was the departure of Amit Singhal, who led Search until 2016 and wrote an internal document arguing Google should limit machine learning specifically so ranking stayed debuggable by human engineers; after he left, ML use "exploded."
**The surprise:** The engineer found and handed off an unfixed, invisible bug that had been silently reordering the top results for 15% of queries since 2015 — and never learned if anyone fixed it.
**The idea:** [Legibility](../../../concepts/legibility.md): keeping a system simple enough for a human to debug is a deliberate constraint someone has to actively defend, and once that person leaves, complexity compounds invisibly.

1 · Hidden reason · Founders · wildcard · [Hacker News](https://news.ycombinator.com/item?id=40133976)

## In depth

In April 2024, journalist Edward Zitron published "The Man Who Killed Google Search," built on internal emails released in the US Department of Justice's antitrust case against Google. The piece traces a 2019 "code yellow" crisis: search-query growth was running behind forecast, and under pressure from the ads and finance side, search lead Ben Gomes (at Google since 1999, before it even sold ads) pushed back hard against proposals to boost engagement in "user-negative ways" — turning off spell-correction, disabling ranking improvements, or sprinkling more results pages with refinements. Gomes was soon replaced by Prabhakar Raghavan, previously the head of ads, effectively ending any firewall between the search team and the revenue team.

The most-upvoted response to Zitron's story, however, came from a different angle entirely. A self-identified ex-Google search engineer, posting as "regw134" on Hacker News, argued the bigger structural loss predated the code-yellow episode: when Amit Singhal left as head of Search in 2016, Google lost the person who had been explicitly fighting "creeping complexity." Singhal had written what the commenter called a "semi-famous" internal document arguing Google should use less machine learning in ranking, or at least contain it, specifically so results stayed interpretable by the humans maintaining them. After he left, the commenter says, every team began launching as many deep-learning projects as it could, the same pattern seen across large tech companies generally.

The commenter's claim is concrete rather than philosophical: older, simpler ranking systems had obvious, visible problems that engineers could spot and fix, while the newer ML-heavy systems accumulate hidden bugs that don't show up in top-line metrics and compound as more complexity gets layered on top. As a direct example, they say they personally discovered an off-by-one error buried in a ranking formula from an old launch — one that had been silently reordering the top results for 15% of all Google queries since 2015 — and handed the finding off when they left the company, with no way of knowing whether it was ever fixed.

Further reading: [Michael Tsai's roundup of the piece and reactions](https://mjtsai.com/blog/2024/05/22/the-man-who-killed-google-search/) · [El País coverage of the DOJ emails](https://english.elpais.com/technology/2024-05-05/the-day-google-started-to-get-worse-we-are-getting-too-close-to-money.html) · [Ed Zitron's newsletter archive](https://www.wheresyoured.at/author/edward/page/12/)

---
id: 2026-11-13-07-most-ad-experiments-cant-prove-anything
number: 7
date: 2026-11-13
title: Most ad experiments can't prove they worked
shape: 2-shocking-number
pool: marketing
concept: statistical-power-blindness
kind: principle
source_link: https://gwern.net/doc/economics/advertising/2015-lewis.pdf
source_name: Lewis & Rao, "The Unfavorable Economics of Measuring the Returns to Advertising," QJE (2015)
strategy: S04
featured: true
wildcard: false
status: [shown]
review: hook 2 · surprise 3 · travels 3
---

# Most ad experiments can't prove they worked

**The find:** Two Yahoo economists analyzed 25 large, real, properly randomized ad experiments run by major retailers and found that in 23 of them, ordinary sales noise was more than 7 times bigger than the ad effect they were trying to measure.
**The surprise:** These weren't sloppy studies — they were big, rigorous, real-money field experiments, and the companies running them still couldn't reliably tell a profitable campaign from a worthless one, because random day-to-day sales swings drowned out the signal.
**The idea:** Having real data and a real experiment doesn't guarantee the result is readable — most measurements are quietly too noisy to answer the question they were built to answer ([Statistical power blindness](../../../concepts/statistical-power-blindness.md)).

2 · Shocking number · Marketing · [Lewis & Rao, QJE](https://gwern.net/doc/economics/advertising/2015-lewis.pdf)

## In depth

In 2013–2015, Yahoo! Research economists Randall A. Lewis and Justin M. Rao circulated a working paper, "On the Near Impossibility of Measuring the Returns to Advertising," presented at the AEA/ASSA 2014 meetings; it was published in the Quarterly Journal of Economics in 2015 under the retitled "The Unfavorable Economics of Measuring the Returns to Advertising" (QJE 130(4): 1941–1973). The two had been given unusual access inside Yahoo to run and publish real advertising experiments at scale. Lewis later moved to Google (eventually Director of Economics there); Rao moved to Microsoft Research, then later to industry roles including Zalando and GBK Collective.

The paper assembled 25 large-scale randomized field experiments run by major US retailers and financial-services/brokerage firms through Yahoo's ad platform between roughly 2007 and 2011, collectively covering about $2.8 million in digital ad spend and typically reaching 500,000 to several million customers per test — genuinely large, properly randomized, real-world campaigns, not toy studies. For each, Lewis and Rao compared the average sales lift the ad was supposed to produce against the standard deviation of individual-level sales, the natural week-to-week noise in how much any customer spends. In 23 of the 25 experiments, that standard deviation was more than seven times larger than the average advertising effect being tested — in the "representative" campaign, detecting a $0.35 per-person sales lift meant working against a roughly $75 per-person standard deviation. That swamping of signal by noise meant the median experiment's 95% confidence interval on ROI was over 100 percentage points wide, and the median campaign would have needed to be roughly 9 times larger just to distinguish break-even from a +50% ROI, and 62 times larger to resolve a 10-point difference. Only 3 of the 25 experiments had adequate statistical power to reliably tell a break-even campaign apart from one actually returning 50%; nine couldn't even statistically rule out the campaign losing all its money. The paper became a foundational reference for the incrementality-testing and media-mix-modeling literature, widely cited as the reason practitioners now combine MMM, geo-lift tests, and holdout experiments rather than trusting any single underpowered lift test.

- [Lewis & Rao 2015, QJE PDF (gwern mirror)](https://gwern.net/doc/economics/advertising/2015-lewis.pdf)
- [Lewis & Rao 2013 AEA working paper (gwern mirror)](https://gwern.net/doc/economics/advertising/2013-lewis.pdf)
- [SSRN abstract page](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=2367103)
- ["Yahoo's Economists Ran 25 Ad Experiments and Could Not Tell Profit From Loss"](https://karandhir.substack.com/p/yahoos-economists-ran-25-ad-experiments)

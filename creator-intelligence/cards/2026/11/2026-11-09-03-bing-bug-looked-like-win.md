---
id: 2026-11-09-03-bing-bug-looked-like-win
number: 3
date: 2026-11-09
title: Bing's bug that looked like a win
shape: 2-shocking-number
pool: marketing
concept: twymans-law
kind: both
source_link: https://exp-platform.com/Documents/2013%20controlledExperimentsAtScale.pdf
source_name: Kohavi et al., "Online Controlled Experiments at Large Scale," KDD 2013
strategy: S16
featured: true
wildcard: false
status: [shown]
review: hook 3 · surprise 3 · travels 3
---

# Bing's bug that looked like a win

**The find:** A 2013 Microsoft experiment shipped a bug that visibly degraded Bing's search results for a test group. The dashboard showed queries per user up more than 10% and ad revenue per user up more than 30%.
**The surprise:** The numbers looked like a huge win because they were real — frustrated users searched more and clicked more ads trying to find what broken results no longer gave them.
**The idea:** [Twyman's Law](../../../concepts/twymans-law.md): any figure that looks interesting or surprisingly good is probably wrong, or measuring the wrong thing.

2 · Shocking number · Marketing · [Kohavi et al., KDD 2013](https://exp-platform.com/Documents/2013%20controlledExperimentsAtScale.pdf)

## In depth

In 2013, Ronny Kohavi's experimentation team at Microsoft — documented in "Online Controlled Experiments at Large Scale" (KDD 2013) and later in his "Trustworthy Online Controlled Experiments: Five Puzzling Outcomes" writeup — ran an A/B test on Bing that shipped with a bug degrading the quality of search results for the treatment group. Nobody caught it by looking at results quality. They caught it by looking at the dashboard, which showed distinct queries per user up more than 10% and revenue per user up more than 30% — numbers so good they would normally be cause for celebration. Investigation found the opposite of success: the algorithm change had made results worse, so users had to search repeatedly to find what they wanted (inflating queries per user) and, failing to find good organic results, clicked on ads instead (inflating ad revenue). The experiment looked like a massive win on the metrics that mattered and was actually a regression that frustrated users were compensating for.

Kohavi, who ran Microsoft's Experimentation Platform (and later was VP and Technical Fellow at Airbnb), used the episode as the canonical illustration of "Twyman's Law": any figure that looks interesting, surprising, or unusually good is probably wrong, or measuring something other than what you think. The law is named for Tony Twyman, a British television and market-research statistician; the earliest written version traces to a 1975 paper by marketing professor A.S.C. Ehrenberg, who credited the maxim to Twyman though Twyman never published it under his own name. Kohavi's team formalized the discipline this incident demanded: before shipping any experiment with a standout result, run sample-ratio-mismatch checks and segment the data by guardrail metrics (page-load latency, crash rates, result relevance) rather than taking the top-line win at face value — a practice later adopted industry-wide at companies including LinkedIn, Booking.com, and Airbnb once they began running controlled experiments at scale.

- [Kohavi, Deng, Frasca, Walker, Xu, Pohlmann — "Online Controlled Experiments at Large Scale," KDD 2013](https://exp-platform.com/Documents/2013%20controlledExperimentsAtScale.pdf)
- [Kohavi — "Trustworthy Online Controlled Experiments: Five Puzzling Outcomes Explained"](https://ai.stanford.edu/~ronnyk/puzzlingOutcomesInControlledExperiments.pdf)
- [Amplitude — "Using Twyman's Law to Avoid Red Herrings in Product Analytics"](https://amplitude.com/blog/twymans-law)
- [Kohavi — "Twyman's Law" slide deck](https://www.exp-platform.com/Documents/TwymansLaw.pdf)

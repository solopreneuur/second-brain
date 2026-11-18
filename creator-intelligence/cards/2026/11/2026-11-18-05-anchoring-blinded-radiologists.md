---
id: 2026-11-18-05-anchoring-blinded-radiologists
number: 5
date: 2026-11-18
title: A random number blinded radiologists
shape: 2-shocking-number
pool: psychology
concept: anchoring
kind: both
source_link: https://doi.org/10.3390/diagnostics12010105
source_name: Diagnostics (Branch, Santana & Hegdé, 2022)
strategy: S14
featured: true
wildcard: false
status: [shown]
review: hook 3 · surprise 3 · travels 3
---

# A random number blinded radiologists

**The find:** Researchers gave practicing radiologists a mammogram to read, along with a number they were told was a prior radiologist's probability estimate for breast cancer — but the number was actually generated at random. With no anchor, the radiologists' diagnostic accuracy averaged around 0.71 (AUC); shown the meaningless random number first, it collapsed to near chance, around 0.46–0.48.
**The surprise:** Trained experts making a life-or-death call let a number they knew nothing about override the actual image in front of them.
**The idea:** Anchoring isn't just a party trick for guessing-game estimates — it can swamp real expertise in exactly the high-stakes settings we assume are anchor-proof ([Anchoring](../../../concepts/anchoring.md)).

2 · Shocking number · Psychology · [Diagnostics, Branch, Santana & Hegdé (2022)](https://doi.org/10.3390/diagnostics12010105)

## In depth

The study, "Biasing Influence of 'Mental Shortcuts' on Diagnostic Decision-Making," was published in the journal Diagnostics in January 2022 by Fallon Branch, Isabella Santana and Jay Hegdé, a neuroscientist at Augusta University's Medical College of Georgia. It ran two linked experiments with practicing radiologists reading real mammogram images with known ground truth (confirmed cancer or no cancer by biopsy). Before each image, radiologists were told a number representing a previous radiologist's probability estimate that the mammogram showed cancer — but the figure was actually produced fresh by a random-number generator for every trial, completely unrelated to the image about to be shown.

Without any such number, the 27 radiologists in the study diagnosed with reasonable skill, averaging around 0.71 on the area-under-curve (AUC) metric commonly used to score diagnostic accuracy — well above chance (0.50). Once a random "prior estimate" was introduced, however, accuracy fell to roughly 0.46–0.48, statistically indistinguishable from a coin flip. The radiologists' own estimates tracked the meaningless number closely, essentially ignoring the mammogram itself. The effect held across both sub-experiments and across radiologists with varying levels of experience, suggesting it wasn't simply a matter of less-skilled readers being more suggestible.

The paper situates this inside the broader anchoring-and-adjustment literature that traces back to Tversky and Kahneman's 1974 work, but makes the case that anchoring in a professional diagnostic setting is a much bigger practical risk than the classic lab demonstrations (estimating UN member counts, wheel-of-fortune number guessing) suggest, because real clinical software — PACS systems, structured reporting templates, AI-assisted triage tools — routinely surfaces prior readings, risk scores, or AI confidence levels to the radiologist before they've formed their own independent judgment. The authors argue this is a design problem as much as a cognitive one: whatever number a system shows first will shape the diagnosis that follows, regardless of whether that number deserves any weight at all.

Further reading: [Full text, PMC](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC8774943/) · [Jay Hegdé's publications page](http://hegde.us/publications/) · [Tversky & Kahneman, "Judgment under Uncertainty: Heuristics and Biases" (1974)](https://www.science.org/doi/10.1126/science.185.4157.1124)

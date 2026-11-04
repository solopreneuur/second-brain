---
id: 2026-11-04-06-autocorrect-slur-dictionary
number: 6
date: 2026-11-04
title: Autocorrect's banned-word dictionary
shape: 1-hidden-reason
pool: founders
concept: ""
kind: observation
source_link: https://www.businessinsider.com/why-iphone-keyboard-autocorrects-ducking-in-texts-explained-2018-9
source_name: Business Insider, interview with Ken Kocienda, 2018
strategy: S02
featured: true
wildcard: false
status: [shown]
review: hook 3 · surprise 3 · travels 2
---

# Autocorrect's banned-word dictionary

**The find:** Ken Kocienda, who wrote the original iPhone autocorrect, says his team had to compile a list of slurs and obscenities and flag them as "never-suggest" entries, so the predictive text engine would never autocorrect a nearby typo into one.
**The surprise:** The inventor of autocorrect's job at points involved curating the worst words in English specifically so the software would know never to suggest them.
**The idea:** The most important design decision in a predictive system is sometimes the explicit list of things it must never predict.

1 · Hidden reason · Founders · [Business Insider, 2018](https://www.businessinsider.com/why-iphone-keyboard-autocorrects-ducking-in-texts-explained-2018-9)

## In depth

Ken Kocienda was principal engineer for iPhone software at Apple, having joined the secret "Project Purple" effort in July 2005. He led design of the first software keyboard and its autocorrection engine, and later wrote about it in his 2018 book "Creative Selection: Inside Apple's Design Process During the Golden Age of Steve Jobs." The slur-blocking story comes from companion interviews he gave Business Insider in September 2018. The mechanism: the iPhone keyboard predicts words by comparing the geometric pattern of where your fingers actually land to the ideal tap-pattern for dictionary words — since letters sit adjacent to other letters, a mistyped word can land closer, pattern-wise, to a different dictionary entry than the one you meant. Because the system would surface whatever dictionary word best matched the tap pattern, Kocienda's team realized typos for innocuous words could occasionally resolve to profanity (he cites "duck," given how close it sits to a swear word on a QWERTY layout). Separately, and more seriously, they found the same proximity logic could surface racial and ethnic slurs as "corrections" for unrelated typos.

Kocienda's fix wasn't a weighting scheme — it was a flagging system: his team compiled "a compendium" of slurs and obscenities and added them into the autocorrect dictionary, but tagged each one with a special marker that made the software treat it as a never-suggest entry, so the predictive engine would never auto-complete or auto-correct into it regardless of pattern proximity. He described the irony plainly: the "ducking" meme people cite as autocorrect's failure is actually the opposite of the slur problem — Apple erred toward blocking profanity and slurs even at the cost of occasionally mangling your actual word, rather than ever letting the system assist in producing one. His book also recounts a 2005 crisis where a keyboard demo for Scott Forstall failed badly, prompting engineer Henri Lamiraux to pull the full team onto the keyboard problem, and Kocienda becoming the "directly responsible individual" under Jobs's and Phil Schiller's exacting demo culture.

- [Business Insider — Kocienda interview on autocorrect and the "ducking" tradeoff](https://www.businessinsider.com/why-iphone-keyboard-autocorrects-ducking-in-texts-explained-2018-9)
- [Business Insider — full Kocienda interview on Apple/Steve Jobs secrecy](https://www.businessinsider.com/ken-kocienda-apple-iphone-steve-jobs-2018-9)
- [Yale Alumni Magazine — Kocienda on the autocorrect dictionary and slur flagging](https://yalealumnimagazine.org/articles/4846-ken-kocienda)
- [Commoncog — case study on the iPhone keyboard's 2005 development crisis](https://commoncog.com/c/cases/the-iphone-keyboard-make-it-or-break-it/)

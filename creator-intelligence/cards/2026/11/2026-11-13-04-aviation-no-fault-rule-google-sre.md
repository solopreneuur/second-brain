---
id: 2026-11-13-04-aviation-no-fault-rule-google-sre
number: 4
date: 2026-11-13
title: Why Google's outage reviews blame no one
shape: 7-far-field
pool: founders
concept: psychological-safety
kind: principle
source_link: https://sre.google/sre-book/postmortem-culture/
source_name: Google SRE Book, "Postmortem Culture"
strategy: S17
featured: true
wildcard: false
status: [shown]
review: hook 3 · surprise 2 · travels 3
---

# Why Google's outage reviews blame no one

**The find:** US aviation crash investigations have run on a legal "no-fault" rule for nearly a century, so pilots and crews will admit the full truth without fear of punishment. Google wrote this exact principle into its own outage-review process by name, and "blameless postmortems" spread across the software industry from there.
**The surprise:** The rule isn't a cultural nicety — it's codified in federal regulation specifically because investigators decided that punishing honesty makes crashes more likely, not less.
**The idea:** If telling the truth about your own error carries a cost, people stop producing the information needed to prevent the next failure ([Psychological safety](../../../concepts/psychological-safety.md)).

7 · Far-field · Founders · [Google SRE Book](https://sre.google/sre-book/postmortem-culture/)

## In depth

American aviation accident investigation has run on a "no-fault" rule for nearly a century, by statute, not just custom. The lineage runs from the Air Commerce Act of 1926 (Commerce Department investigates causes) through the Civil Aeronautics Board's Bureau of Aviation Safety (1940), to the creation of the NTSB inside the new Department of Transportation in 1967, to the Independent Safety Board Act of 1974, which spun the NTSB out as a fully independent agency on the reasoning that "no Federal agency can properly perform such functions unless it is totally separate and independent from any other agency." The no-fault rule itself is codified: 49 CFR § 831.4(c) states NTSB investigations "are fact-finding proceedings with no adverse parties" and are "not conducted for the purpose of determining the rights, liabilities, or blame of any person or entity." A companion statute, 49 U.S.C. § 1154(b), bars NTSB probable-cause findings from being admitted as evidence in civil lawsuits. The mechanism is explicit: investigators reason that pilots, controllers, and mechanics will only disclose the full chain of errors — their own included — if nothing they say can be used to punish or sue them; strip out that fear and the data gets richer and the next crash gets prevented.

Google's Site Reliability Engineering book (sre.google/sre-book, published 2016) imports this logic by name in its "Postmortem Culture" chapter, written by John Lunney and Sue Lueder and edited by Gary O'Connor. It traces the blameless concept to "healthcare and avionics industries where mistakes can be fatal," arguing those fields "nurture an environment where every 'mistake' is seen as an opportunity to strengthen the system," and that without this, "people will not bring issues to light for fear of punishment."

The phrase's path into software specifically runs through John Allspaw, then CTO of Etsy, who published "Blameless PostMortems and a Just Culture" on Etsy's Code as Craft blog in May 2012 — four years before the SRE book. Allspaw drew on Sidney Dekker's "Just Culture" research and framed the goal as understanding "how it made sense for someone to do what they did," since "they thought what they were doing made sense" at the time. That post is widely credited as the entry point that carried the aviation-derived term into mainstream tech practice before Google's book cemented it industry-wide.

- [Google SRE Book — Postmortem Culture](https://sre.google/sre-book/postmortem-culture/)
- [49 CFR § 831.4 — Cornell Law](https://www.law.cornell.edu/cfr/text/49/831.4)
- [Wikipedia — Independent Safety Board Act of 1974](https://en.wikipedia.org/wiki/Independent_Safety_Board_Act_of_1974)
- [Wikipedia — National Transportation Safety Board](https://en.wikipedia.org/wiki/National_Transportation_Safety_Board)

---
id: 2026-11-15-06-disney-infrared-face-tracking
number: 6
date: 2026-11-15
title: Disney filmed 16 million faces
shape: 2-shocking-number
pool: marketing
concept: ""
kind: observation
source_link: https://qz.com/1039102/disney-can-now-use-infrared-cameras-to-track-your-reactions-to-films-in-darkened-cinemas
source_name: Quartz
strategy: S04
featured: true
wildcard: true
status: [shown]
review: hook 3 · surprise 3 · travels 2
---

# Disney filmed 16 million faces

**The find:** Disney Research rigged a 400-seat theater with infrared cameras and filmed 3,179 moviegoers across 150 screenings, capturing 16 million facial data points to train an AI that predicts a viewer's reactions for the rest of a film after watching just their face for a few minutes.
**The surprise:** The system didn't just score whether a scene landed — it could flag which individual viewers were reacting differently from everyone else around them, in real time, in the dark.
**The idea:** A few minutes of someone's face is enough data to predict how the rest of their experience will go.

2 · Shocking number · Marketing · wildcard · [Quartz](https://qz.com/1039102/disney-can-now-use-infrared-cameras-to-track-your-reactions-to-films-in-darkened-cinemas)

## In depth

In 2015 and 2016, Disney Research instrumented a 400-seat theater with four infrared cameras and infrared illuminators mounted above the screen, filming audiences in the dark across 150 screenings of nine films, including "Big Hero 6," "The Jungle Book," "Zootopia," and "Star Wars: The Force Awakens." The cameras captured 3,179 moviegoers' faces, generating roughly 16 million facial landmark data points. Researchers Zhiwei Deng and Greg Mori (Simon Fraser University), Rajitha Navarathna, Peter Carr, Stephan Mandt, and Iain Matthews (Disney Research), and Yisong Yue (Caltech) used this dataset to build "factorized variational autoencoders" (FVAEs), published at CVPR 2017.

FVAEs work like a recommendation engine for faces: rather than linearly factoring expressions the way older tensor methods did, a deep neural network learns a compressed, nonlinear representation of each face's expression over time, decomposing it into a stereotypical audience-wide reaction curve plus an individual deviation from it. After watching just a few minutes of someone's face, the model could predict their expressions, smiles, laughs, grimaces, for the rest of the runtime, and could flag individual viewers whose reactions diverged from the crowd average. The paper framed this as a tool to measure, moment by moment, whether a scene was landing as intended — instrumented test screenings replacing clipboard surveys with continuous facial data.

There's no indication moviegoers were told cameras were tracking their faces beyond standard test-screening consent forms; reporting at the time flagged the lack of disclosed, specific consent for facial analysis as a concern. No evidence has surfaced that Disney deployed FVAEs commercially in theaters or editing pipelines afterward; it remains a published research artifact, though a later Disney patent covers "characterizing audience engagement based on emotional alignment with characters," suggesting continued internal interest. Commercially, companies like Realeyes and Affectiva (now part of Smart Eye) already sell facial-coding ad-testing services, using opt-in webcam footage of viewers watching commercials to score attention and emotion for advertisers — a lighter-touch, consent-based cousin of Disney's theater experiment.

Further reading: [CVPR 2017 paper, PDF](https://openaccess.thecvf.com/content_cvpr_2017/papers/Deng_Factorized_Variational_Autoencoders_CVPR_2017_paper.pdf) · [Disney Research publication page](https://la.disneyresearch.com/publication/factorized-variational-autoencoder/) · [EurekAlert coverage](https://www.eurekalert.org/news-releases/915985)

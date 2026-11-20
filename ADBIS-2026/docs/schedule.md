---
layout: default
title: Schedule
nav_order: 2
---

The tutorial is a **90-minute session** at [ADBIS 2026](https://adbis26.sciencesconf.org/) in Orléans, France. The exact day, time, and room will be announced on this page once the conference programme is finalised.

The session combines a conceptual presentation with a practical demonstration, and is delivered in person by Ali Ismail-Fawaz, Germain Forestier, and Antoine Guillaume. The speakers will be available afterwards for Q&A, and questions are always welcome on the [_aeon_ Discord](https://discord.gg/GEE6PCfJwf) or via email.

We will try to get all slides and accompanying code examples uploaded before the tutorial. If we are unable to, we will upload them after.

The session is organised in three parts (times are given relative to the session start):

## Part 1 — Concepts (≈ 60 minutes)

- **Introduction to time series machine learning** — what time series classification (TSC) and regression (TSER) are, and the role of deep learning for sequential data. _(00:00)_

- **Overview of the _aeon_ toolkit** — design principles, the unified `fit`/`predict` interface, and how _aeon_ simplifies the use of advanced algorithms for sequential data. _(00:15)_

- **Deep learning architectures for time series** — the intuition behind convolutional (FCN), residual (ResNet), multi-scale (Inception/LITE), and hybrid models, and their strengths for modelling univariate and multivariate temporal data. _(00:30)_

  [Slides](https://github.com/aeon-tutorials/ADBIS-2026/tree/main/Slides) _(to be uploaded)_

## Part 2 — Hands-on coding demonstration (≈ 20 minutes)

- **Using deep learning models in _aeon_** — loading benchmark datasets, configuring a neural model, training estimators, and evaluating predictions for both classification and regression. _(01:00)_

  [Notebook (file)](https://github.com/aeon-tutorials/ADBIS-2026/blob/main/Notebooks/rehab_pile_deep_learning.ipynb) — see also the [Slides & Code](code.html) page.

## Part 3 — Application & Q&A (≈ 10 minutes)

- **Application: skeleton-based rehabilitation with Rehab-Pile** — how skeleton motion sequences can be formatted as multivariate time series and used with deep learning models in _aeon_ for movement assessment in healthcare. _(01:20)_

- **Questions & discussion** — an open Q&A to discuss specific use cases and clarify technical details. _(01:25)_

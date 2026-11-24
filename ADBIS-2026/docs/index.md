---
layout: default
title: Home
header: Deep Learning for Time Series with aeon
nav_order: 1
---

## Overview

We present a tutorial on **deep learning for time series classification and regression** with [_aeon_](https://www.aeon-toolkit.org), a Python library dedicated to time series machine learning. The tutorial first introduces the _aeon_ toolkit and its unified interface, before focusing on neural architectures tailored to sequential data. We describe how participants will train and evaluate deep learning models for both classification and regression tasks using the [_scikit-learn_](https://scikit-learn.org/)-compatible API.

In addition, we highlight a practical application in **skeleton-based rehabilitation motion assessment**, where deep models are applied to multivariate motion sequences from the Rehab-Pile archive. This application demonstrates how learned representations can support real-world healthcare scenarios involving movement analysis and assessment.

_Keywords: Time series · Deep learning · Classification · Regression · Rehabilitation · aeon_

## When & Where

- Conference: [ADBIS 2026](https://adbis26.sciencesconf.org/) — 30th European Conference on Advances in Databases and Information Systems
- Dates: 28 September – 1 October 2026
- Location: Orléans, France
- Session: 90-minute tutorial (exact day, time, and room to be announced)

## Prerequisites

This tutorial is intended for researchers and practitioners working in data science and machine learning who are interested in temporal or sequential data. It is particularly relevant for those who wish to apply deep learning techniques to time series problems in domains such as healthcare, sensor analysis, or human motion understanding.

- A basic understanding of machine learning concepts
- Familiarity with Python programming
- Prior exposure to deep learning or time series analysis is beneficial, but **not** strictly required — the tutorial introduces the necessary concepts before moving to practical examples.

## Background

Time series data \[[14](https://doi.org/10.1007/s10618-024-01022-1)\] appears in many scientific and industrial contexts, ranging from biomedical signals to sensor recordings and financial measurements. While traditional machine learning approaches remain relevant, deep learning methods \[[11](https://doi.org/10.1007/s10618-019-00619-1),[15](https://doi.org/10.1145/3649448)\] have gained significant traction due to their ability to automatically learn hierarchical representations directly from raw sequences.

**Time series classification (TSC)** assigns categorical labels to sequences, whereas **time series regression (TSER)** \[[6](https://doi.org/10.1007/s10618-023-00963-3)\] predicts continuous outcomes. Both tasks benefit from neural architectures such as convolutional neural networks (CNNs), residual networks, and hybrid approaches designed to capture temporal dependencies and spatial structure.

_aeon_ \[[13](https://www.aeon-toolkit.org)\] is an open-source Python library designed for time series machine learning. It provides a unified interface for a wide range of learning tasks on sequential data, including classification, regression, clustering, forecasting, anomaly detection, segmentation, and similarity search. The toolkit follows the design principles of _scikit-learn_ \[[16](https://www.jmlr.org/papers/v12/pedregosa11a.html)\], exposing a consistent estimator API based on the `fit` and `predict` paradigm, which allows integration with existing machine learning workflows.

The deep learning module of _aeon_ includes several neural architectures that have been adapted for time series data. These include convolutional models such as **Fully Convolutional Networks (FCN)**, which learn local temporal patterns, and **Residual Networks (ResNet)** \[[17](https://doi.org/10.1109/IJCNN.2017.7966039)\], which enable the training of deeper models through skip connections. More recent architectures, such as **Inception**-based models \[[12](https://doi.org/10.1007/s10618-020-00710-y),[7](https://doi.org/10.1109/DSAA60987.2023.10302569),[9](https://doi.org/10.1007/s41060-024-00657-z)\], capture patterns at multiple temporal scales, while hybrid approaches \[[10](https://doi.org/10.1109/BigData55660.2022.10020496),[1](https://doi.org/10.1109/BigData62323.2024.10825473)\] combine different architectural components to improve representation learning. These models support multivariate sequences \[[2](https://arxiv.org/abs/1811.00075)\] and can leverage hardware acceleration when available.

The tutorial concludes with a domain-specific application on skeleton-based human motion rehabilitation using the **Rehab-Pile** archive \[[8](https://arxiv.org/abs/2507.21018)\]. This example illustrates how the presented methods can be applied to real-world motion data and highlights the challenges and opportunities associated with rehabilitation-oriented time series analysis.

## References

\[[1](https://doi.org/10.1109/BigData62323.2024.10825473)\] O. Badi, M. Devanne, __A. Ismail-Fawaz__, J. Abdullayev, V. Lemaire, S. Berretti, __J. Weber__, and __G. Forestier__. CoCaLite: A hybrid model combining catch22 and LITE for time series classification. _IEEE International Conference on Big Data (BigData)_, 1229–1236, 2024.

\[[2](https://arxiv.org/abs/1811.00075)\] __A. Bagnall__, H. A. Dau, J. Lines, M. Flynn, J. Large, A. Bostrom, P. Southam, and E. Keogh. The UEA multivariate time series classification archive, 2018. _arXiv:1811.00075_, 2018.

\[[3](https://doi.org/10.1145/3637528.3671443)\] __A. Bagnall__, M. Middlehurst, __G. Forestier__, __A. Ismail-Fawaz__, __A. Guillaume__, D. Guijo-Rubio, C. W. Tan, A. Dempster, and G. I. Webb. A hands-on introduction to time series classification and regression. _Proceedings of the 30th ACM SIGKDD Conference on Knowledge Discovery and Data Mining_, 6410–6411, 2024.

\[[6](https://doi.org/10.1007/s10618-023-00963-3)\] D. Guijo-Rubio, M. Middlehurst, G. Arcencio, D. F. Silva, and __A. Bagnall__. Unsupervised feature based algorithms for time series extrinsic regression. _Data Mining and Knowledge Discovery_, 2023.

\[[7](https://doi.org/10.1109/DSAA60987.2023.10302569)\] __A. Ismail-Fawaz__, __M. Devanne__, S. Berretti, __J. Weber__, and __G. Forestier__. LITE: Light inception with boosting techniques for time series classification. _IEEE International Conference on Data Science and Advanced Analytics (DSAA)_, 1–10, 2023.

\[[8](https://arxiv.org/abs/2507.21018)\] __A. Ismail-Fawaz__, __M. Devanne__, S. Berretti, __J. Weber__, and __G. Forestier__. Deep learning for skeleton based human motion rehabilitation assessment: A benchmark. _arXiv:2507.21018_, 2025.

\[[9](https://doi.org/10.1007/s41060-024-00657-z)\] __A. Ismail-Fawaz__, __M. Devanne__, S. Berretti, __J. Weber__, and __G. Forestier__. Look into the LITE in deep learning for time series classification. _International Journal of Data Science and Analytics_, 20(4):4029–4049, 2025.

\[[10](https://doi.org/10.1109/BigData55660.2022.10020496)\] __A. Ismail-Fawaz__, __M. Devanne__, __J. Weber__, and __G. Forestier__. Deep learning for time series classification using new hand-crafted convolution filters. _IEEE International Conference on Big Data (Big Data)_, 972–981, 2022.

\[[11](https://doi.org/10.1007/s10618-019-00619-1)\] H. Ismail Fawaz, __G. Forestier__, __J. Weber__, L. Idoumghar, and P.-A. Muller. Deep learning for time series classification: a review. _Data Mining and Knowledge Discovery_, 33(4):917–963, 2019.

\[[12](https://doi.org/10.1007/s10618-020-00710-y)\] H. Ismail Fawaz, B. Lucas, __G. Forestier__, C. Pelletier, D. F. Schmidt, __J. Weber__, G. I. Webb, L. Idoumghar, P.-A. Muller, and F. Petitjean. InceptionTime: Finding AlexNet for time series classification. _Data Mining and Knowledge Discovery_, 34(6):1936–1962, 2020.

\[[13](https://www.aeon-toolkit.org)\] M. Middlehurst, __A. Ismail-Fawaz__, __A. Guillaume__, C. Holder, D. Guijo-Rubio, G. Bulatova, L. Tsaprounis, L. Mentel, M. Walter, P. Schäfer, et al. aeon: a Python toolkit for learning from time series. _Journal of Machine Learning Research_, 25(289):1–10, 2024.

\[[14](https://doi.org/10.1007/s10618-024-01022-1)\] M. Middlehurst, P. Schäfer, and __A. Bagnall__. Bake off redux: a review and experimental evaluation of recent time series classification algorithms. _Data Mining and Knowledge Discovery_, 38(4):1958–2031, 2024.

\[[15](https://doi.org/10.1145/3649448)\] N. Mohammadi Foumani, L. Miller, C. W. Tan, G. I. Webb, __G. Forestier__, and M. Salehi. Deep learning for time series classification and extrinsic regression: A current survey. _ACM Computing Surveys_, 56(9):1–45, 2024.

\[[17](https://doi.org/10.1109/IJCNN.2017.7966039)\] Z. Wang, W. Yan, and T. Oates. Time series classification from scratch with deep neural networks: A strong baseline. _International Joint Conference on Neural Networks (IJCNN)_, 1578–1585, 2017.

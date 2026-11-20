---
layout: default
title: Slides & Code
nav_order: 3
---

#### __\*\* UNDER CONSTRUCTION \*\*__

This tutorial makes use of the [_aeon_ toolkit](https://www.aeon-toolkit.org/) for its code examples. _aeon_ is an open source, _scikit-learn_ compatible framework for time series machine learning. The hands-on part demonstrates how deep learning models can be trained using the same `fit`/`predict` workflow as any other estimator in _aeon_.

The coding demonstration is provided as a Jupyter notebook covering both **classification** and **regression** with deep learning models. The notebook and slides are available on this [GitHub repository](https://github.com/aeon-tutorials/ADBIS-2026) and will be finalised before the tutorial.

- Deep learning for classification & regression — [Notebook (file)](https://github.com/aeon-tutorials/ADBIS-2026/blob/main/Notebooks/rehab_pile_deep_learning.ipynb) & [Notebook (Google Colab)](https://colab.research.google.com/github/aeon-tutorials/ADBIS-2026/blob/main/Notebooks/rehab_pile_deep_learning.ipynb) & [Slides](https://github.com/aeon-tutorials/ADBIS-2026/tree/main/Slides) _(to be uploaded)_

You can also launch the notebooks interactively in your browser without any local installation:

[![binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/aeon-tutorials/ADBIS-2026/main) [![nbviewer](https://raw.githubusercontent.com/jupyter/design/master/logos/Badges/nbviewer_badge.svg)](https://nbviewer.org/github/aeon-tutorials/ADBIS-2026/tree/main/Notebooks/)

### Quick start

The two examples below summarise the workflow shown during the live demonstration. To run them locally, install _aeon_ with `pip install -U aeon`.

**Classification** — train a Fully Convolutional Network and produce class probability estimates:

```python
from aeon.datasets import load_classification
from aeon.classification.deep_learning import FCNClassifier

X, y = load_classification("ArrowHead", split="TRAIN")
X_test, _ = load_classification("ArrowHead", split="TEST")

clf = FCNClassifier(n_epochs=50, batch_size=16)
clf.fit(X, y)

probs = clf.predict_proba(X_test)
```

**Regression** — train a Residual Network and produce continuous predictions:

```python
from aeon.datasets import load_regression
from aeon.regression.deep_learning import ResNetRegressor

X, y = load_regression("BarCrawl6min", split="TRAIN")
X_test, _ = load_regression("BarCrawl6min", split="TEST")

reg = ResNetRegressor(n_epochs=50, batch_size=16)
reg.fit(X, y)

preds = reg.predict(X_test)
```

<img src="images/logo/aeon.png" alt="aeon logo" width="400"/>

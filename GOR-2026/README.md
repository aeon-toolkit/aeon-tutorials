# An Introduction to Time Series Machine Learning with aeon

## GOR 2026 tutorial, Hamburg, 26 November 2026

[![nbviewer](https://raw.githubusercontent.com/jupyter/design/master/logos/Badges/nbviewer_badge.svg)](https://nbviewer.org/github/aeon-toolkit/aeon-tutorials/tree/main/GOR-2026/Notebooks/)

Presented by Tony Bagnall (University of Southampton), Ali Ismail-Fawaz (Université de Haute-Alsace)
and Antoine Guillaume (Novahé).

This tutorial introduces machine learning from time series with the
[_aeon_ toolkit](https://www.aeon-toolkit.org/), an open source, _scikit-learn_ compatible
framework for time series machine learning. It builds on the tutorials we gave at KDD 2024 and
ECML-PKDD 2024, updated for _aeon_ 1.6.0.

Questions about _aeon_ are always welcome on the [_aeon_ Discord](https://discord.gg/D6rzqHGKRJ).

## Contents

| Part | Topic | Notebook | Slides |
|------|-------|----------|--------|
| 1 | Introduction to time series machine learning | [part1_introduction](Notebooks/part1_introduction.ipynb) ([Colab](https://colab.research.google.com/github/aeon-toolkit/aeon-tutorials/blob/main/GOR-2026/Notebooks/part1_introduction.ipynb)) | [pptx](Slides/part1_introduction.pptx) |
| 2 | Classification and regression | [part2_classification_regression](Notebooks/part2_classification_regression.ipynb) ([Colab](https://colab.research.google.com/github/aeon-toolkit/aeon-tutorials/blob/main/GOR-2026/Notebooks/part2_classification_regression.ipynb)) | [pptx](Slides/part2_classification_regression.pptx) |
| 3 | Clustering | [part3_clustering](Notebooks/part3_clustering.ipynb) ([Colab](https://colab.research.google.com/github/aeon-toolkit/aeon-tutorials/blob/main/GOR-2026/Notebooks/part3_clustering.ipynb)) | [pptx](Slides/part3_clustering.pptx) |
| 4 | Similarity search | [part4_similarity_search](Notebooks/part4_similarity_search.ipynb) ([Colab](https://colab.research.google.com/github/aeon-toolkit/aeon-tutorials/blob/main/GOR-2026/Notebooks/part4_similarity_search.ipynb)) | [pptx](Slides/part4_similarity_search.pptx) |
| 5 | Segmentation | [part5_segmentation](Notebooks/part5_segmentation.ipynb) ([Colab](https://colab.research.google.com/github/aeon-toolkit/aeon-tutorials/blob/main/GOR-2026/Notebooks/part5_segmentation.ipynb)) | [pptx](Slides/part5_segmentation.pptx) |
| 6 | Anomaly detection | [part6_anomaly_detection](Notebooks/part6_anomaly_detection.ipynb) ([Colab](https://colab.research.google.com/github/aeon-toolkit/aeon-tutorials/blob/main/GOR-2026/Notebooks/part6_anomaly_detection.ipynb)) | [pptx](Slides/part6_anomaly_detection.pptx), [pdf](Slides/part6_anomaly_detection.pdf) |
| 7 | Deep learning models in _aeon_ | [part7_deep_learning_based](Notebooks/part7_deep_learning_based.ipynb) ([Colab](https://colab.research.google.com/github/aeon-toolkit/aeon-tutorials/blob/main/GOR-2026/Notebooks/part7_deep_learning_based.ipynb)) | [pdf](Slides/part7_deep_learning.pdf) |
| 7 | Deep learning case study: rehabilitation exercise assessment (Rehab-Pile) | [part7_deep_learning_rehab_pile](Notebooks/part7_deep_learning_rehab_pile.ipynb) ([Colab](https://colab.research.google.com/github/aeon-toolkit/aeon-tutorials/blob/main/GOR-2026/Notebooks/part7_deep_learning_rehab_pile.ipynb)) | [pdf](Slides/part7_deep_learning_rehab_pile.pdf) ([LaTeX source](Slides/part7_deep_learning_rehab_pile/)) |
| 8 | Conclusions and future directions | | [pptx](Slides/part8_conclusion.pptx) |

The notebooks are stored with their outputs, so you can read them on GitHub or
[nbviewer](https://nbviewer.org/github/aeon-toolkit/aeon-tutorials/tree/main/GOR-2026/Notebooks/)
without running anything.

## Running the code

Each notebook starts with a cell that installs what it needs, for example

```bash
pip install aeon==1.6.0 matplotlib seaborn
```

so the notebooks run as they are on Google Colab (links in the table) or in a fresh local
environment. Use Python 3.11 to 3.13: _aeon_ 1.6.0 supports Python 3.11 to 3.14, but TensorFlow,
which the deep learning examples in parts 2 and 7 need, is not available for Python 3.14 yet.

Datasets that do not ship with _aeon_ are downloaded the first time a notebook runs.

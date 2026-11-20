# Slides

Beamer source of the ADBIS 2026 tutorial deck (39 frames, 16:9).

- `main.tex`: the slides. `aeontheme.tex`: colours, frame title, footline, code style.
- `figures/`: PDF figures written by `Notebooks/rehab_pile_deep_learning.ipynb` (copy them again after re-running the notebook).
- `images/`: the aeon logo.

**Overleaf**: upload this folder as a zip (New Project > Upload Project). The compiler is pdfLaTeX and the main document is `main.tex`. Only standard packages are used (beamer, TikZ, listings, booktabs, lmodern).

**Locally**: `pdflatex main.tex`, twice for the frame count.

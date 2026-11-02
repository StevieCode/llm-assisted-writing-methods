# LLM-assisted writing: methods documentation

Companion methods for **LLM assisted writing deserves empirical evaluation**, by Xuan Zhong Feng, Yi Lin, Yiye Zhang, Chunhua Weng, and Yifan Peng.

## Read the methods

- [Methods in Markdown](METHODS.md): complete methods, with navigable headings, equations, country lists, and references.
- [Methods PDF](methods.pdf): typeset reading copy.
- [Supplementary Information](supplementary-information.pdf): the existing supplementary tables and prompts cited by the methods.
- [Methods source](methods-body.tex), [standalone TeX wrapper](methods.tex), and [bibliography](references.bib): editable source and references.

The Methods section was relocated from the revised manuscript to keep the manuscript in Comment format. The complete source text is preserved verbatim in `methods-body.tex`; the Markdown changes presentation only. The supplementary PDF is an unchanged copy of the accompanying manuscript supplement. This repository contains documentation, not analysis code, trained models, or underlying datasets.

## Reviewer navigation

- Classifier training, calibration, and cohort assignment: [Identification of LLM-assisted writing](METHODS.md#identification-of-llm-assisted-writing).
- Semantic embeddings and topic mapping: [Feature extraction](METHODS.md#feature-extraction).
- Reference-list and citation measures: [Outcome measures](METHODS.md#outcome-measures).
- Journal access classification and sensitivity analyses: [Journal access model](METHODS.md#journal-access-model).
- Statistical comparisons and multiplicity adjustment: [Statistical analysis](METHODS.md#statistical-analysis).

## Build the PDF

With a TeX distribution providing the packages in `methods.tex` and the `naturemag` bibliography style:

```sh
pdflatex methods.tex
bibtex methods
pdflatex methods.tex
pdflatex methods.tex
```

Documentation snapshot: 2 November 2026.

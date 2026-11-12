# Research Statement

[![Build and publish](https://github.com/inoue0426/research_statement/actions/workflows/publish.yml/badge.svg)](https://github.com/inoue0426/research_statement/actions/workflows/publish.yml)

Public research statement for **Yoshitaka Inoue**.

## Research vision

**From predictive biological modeling to mechanism-guided therapeutic discovery.**

I develop computational methods to predict biological responses, discover causal mechanisms underlying treatment sensitivity and resistance, understand when those mechanisms are shared or context-dependent, and use the resulting insights to guide therapeutic intervention design.

**Identifiability** (what mechanisms can be supported by the available data and experiments) and **transferability** (when mechanisms remain valid across contexts) are equally important to this program. The initial biological focus is pan-cancer drug response and tumor microenvironments.

**Last updated: November 2026**

Published version: <https://inoue0426.github.io/research_statement/>

## Research directions

1. **Mechanism-aware intervention modeling** — connecting drugs and genetic perturbations to targets, regulatory pathways, and treatment-induced cellular changes.
2. **Context-aware mechanism discovery** — combining molecular states, cell–cell communication, and spatial tumor-microenvironment information to distinguish shared and context-specific mechanisms.
3. **Identifiability, transferability, and reliable inference** — evaluating mechanistic ambiguity, cross-context validity, and evidence-supported predictions, including when to defer or request more data.

## Five-year and ten-year goals

- **Five years:** Establish an independent computational research program in mechanism-aware cancer drug-response modeling and experimentally validated mechanism discovery, with sustained experimental collaborations.
- **Ten years:** Lead a large interdisciplinary research program spanning machine learning, computational biology, experimental cancer biology, and therapeutic discovery. Connect predictive modeling and causal validation to both optimization of existing therapies and discovery of novel therapeutic interventions.

These are future research aims, not claims of completed causal discoveries or validated therapies.

## Selected work

### PerturbRx
**PerturbRx: Learning Treatment-Conditioned Latent Transitions for Patient Drug Response Prediction**

Models treatment- and dose-conditioned latent changes from single-cell perturbation data and evaluates their use for patient-level treatment-response prediction. The program's next step is to test their added value against simple baselines and study which mechanistic conclusions can actually be identified and transferred.

- [Preprint](https://arxiv.org/abs/2608.21349)

### drGT
**drGT: Interpretable Drug Response Prediction with Attention-Guided Gene Attribution on a Drug-Cell-Gene Heterogeneous Graph**

A heterogeneous drug–cell–gene graph model for treatment-response prediction with gene-level attribution. Published in *BMC Bioinformatics*.

- [Paper](https://doi.org/10.1186/s12859-026-06417-z)
- [Code](https://github.com/sciluna/drGT)

### DrugAgent
**DrugAgent: Reliable Multi-Agent Integration of Conflicting Biomedical Evidence for Drug-Target Interaction Assessment**

A multi-agent framework for integrating machine-learning, knowledge-graph, and literature evidence for biomedical interaction assessment.

- [Preprint](https://arxiv.org/abs/2408.13378)
- [Code](https://github.com/sciluna/DrugAgent)

### Additional research foundations

- **BiGCN** (bioRxiv, 2024): bi-graph convolution for single-cell transcriptome imputation.
- **GraphPINE** (ICLR 2025 Workshop on Machine Learning for Genomics Explorations): interpretable graph importance propagation for drug response prediction.
- **CellMinerCDB v2.2** (*Nucleic Acids Research*, 2026): cross-database cancer-cell-line pharmacogenomics resource.
- **Drug discovery in the era of artificial intelligence** (*Health Data Science*, 2026): review of AI methods spanning target identification to clinical trials.

These publications complement the selected projects above; PerturbRx is already listed as a preprint, rather than a peer-reviewed journal article.

## Source and build

The statement is written in LaTeX:

- `main.tex` — research statement
- `references.bib` — bibliography
- `main.pdf` — generated PDF (may lag behind the source until the build workflow runs)

To build locally:

```bash
pdflatex main.tex
bibtex main
pdflatex main.tex
pdflatex main.tex
```

More about my research: [inoue0426.github.io](https://inoue0426.github.io/).

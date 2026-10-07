# Research Statement

[![Build and publish](https://github.com/inoue0426/research_statement/actions/workflows/publish.yml/badge.svg)](https://github.com/inoue0426/research_statement/actions/workflows/publish.yml)

Public research statement for **Yoshitaka Inoue**.

My research focuses on machine learning for therapeutic intervention and biological dynamics: learning how treatments change biological systems, transferring those representations across experimental and patient contexts, and identifying when mechanistic evidence is strong enough to support a prediction.

**Last updated: October 2026**

Published version: <https://inoue0426.github.io/research_statement/>

## Research directions

- **Intervention-conditioned representations** — learning treatment-induced state transitions from perturbational data and transferring them toward patient-level treatment-response prediction.
- **Biological context for transfer** — studying how spatial structure, cell states, and cell–cell communication affect whether a treatment mechanism transfers across systems.
- **Mechanism-of-action and evidence-aware reasoning** — integrating predictive, structured, and literature evidence while making conflict, missing evidence, and abstention explicit.

## Selected work

### PerturbRx
**PerturbRx: Learning Treatment-Conditioned Latent Transitions for Patient Drug Response Prediction**

Learns treatment- and dose-conditioned latent transitions from single-cell perturbation data and transfers them to pretreatment patient profiles for treatment-response prediction.

- [Preprint](https://arxiv.org/abs/2608.21349)

### drGT
**drGT: Interpretable Drug Response Prediction with Attention-Guided Gene Attribution on a Drug-Cell-Gene Heterogeneous Graph**

A heterogeneous drug–cell–gene graph model for treatment-response prediction with gene-level, mechanism-oriented attribution. Published in *BMC Bioinformatics*.

- [Paper](https://doi.org/10.1186/s12859-026-06417-z)
- [Code](https://github.com/sciluna/drGT)

### DrugAgent
**DrugAgent: Reliable Multi-Agent Integration of Conflicting Biomedical Evidence for Drug-Target Interaction Assessment**

A multi-agent framework for integrating machine-learning, knowledge-graph, and literature evidence for biomedical interaction assessment.

- [Preprint](https://arxiv.org/abs/2408.13378)
- [Code](https://github.com/sciluna/DrugAgent)

## Source

The statement is written in LaTeX:

- `main.tex` — research statement
- `references.bib` — bibliography

## Build

A standard LaTeX + BibTeX build is sufficient:

```bash
pdflatex main.tex
bibtex main
pdflatex main.tex
pdflatex main.tex
```

## About

More about my research and publications: [inoue0426.github.io](https://inoue0426.github.io/)

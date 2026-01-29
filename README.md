# Multi-Scale Forecasting of Citi Bike Demand in New York City — Appendices and Reproducible Workflow

This repository contains Appendices A–F and supporting Python/Jupyter Notebook workflow materials for the master’s dissertation:

**Multi-Scale Forecasting of Citi Bike Demand in New York City: Including Time Series, Machine Learning, and Deep Learning Models**  
Zoltan Jelovich (2026)

## Contents
- `appendices/`: Appendix Markdown files and supplementary figures (A–F)
- `notebooks/`: Reproducible workflow notebooks (ordered)
- `src/`: Reusable Python modules used by notebooks
- `docs/`: Data source notes and reproducibility instructions

## How to cite
See `CITATION.cff`. Please cite the dissertation and (if used) this repository release.

## Licensing
- Code (notebooks, `src/`): see `LICENSE-CODE`
- Written appendix materials (PDFs, figures/tables you created): see `LICENSE-TEXT`

## Reproducibility (high level)
1. Create the environment (choose one):
   - `conda env create -f environment.yml`
   - or `pip install -r requirements.txt`
2. Follow `docs/data_sources.md` to obtain required datasets.
3. Run notebooks in `notebooks/` in numeric order.

## Data note
This repo does not include raw Citi Bike trip data or other large/raw source datasets. See `docs/data_sources.md`.

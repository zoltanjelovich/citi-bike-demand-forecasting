# Multi-Scale Forecasting of Citi Bike Demand in New York City  
## Appendices and Reproducible Workflow

This repository contains supplementary materials for the master’s dissertation:

Multi-Scale Forecasting of Citi Bike Demand in New York City: Including Time Series, Machine Learning, and Deep Learning Models  
Zoltan Jelovich (2026)

Due to page-length constraints, all appendices (Appendices A–F), including supplementary figures, tables, extended methodological details, and code notebooks, are provided here.

## Repository contents

- `appendices/`  
  Markdown appendices corresponding to Appendices A–F referenced in the dissertation text.  
  See `appendices/README.md` for an index mapping appendix letters to files.

- `notebooks/`  
  Jupyter Notebook (`.ipynb`) files documenting the analytical workflow, including:
  - data preparation and aggregation
  - feature construction
  - model estimation and evaluation
  - interpretability and sensitivity analyses  

  Notebooks are numbered to indicate their intended execution order.

## Scope and data availability

This repository **does not include raw or processed datasets**, including Citi Bike trip records or external contextual datasets (e.g., weather, environmental, or built-environment data).

All notebooks assume that required datasets have been obtained separately from their original public sources and placed in user-defined local directories. File paths and assumptions are documented within the notebooks themselves.

## Reproducibility notes

- The notebooks reflect the workflow and outputs as submitted with the dissertation.
- Time-ordered train/validation/test splits and leakage controls are implemented explicitly within the notebooks.
- Results are intended to support transparency and methodological reproducibility rather than turnkey execution.

## Citation

If you reference or reuse materials from this repository, please cite the dissertation:

> Jelovich, Z. (2026). *Multi-Scale Forecasting of Citi Bike Demand in New York City: Including Time Series, Machine Learning, and Deep Learning Models*. Master’s dissertation.

Citation metadata is also provided in `CITATION.cff`.

## Licensing

- Code and Jupyter notebooks are licensed under the MIT License (see `LICENSE`).
- Appendix materials (Markdown files, figures, tables, and written content) are licensed under  
  Creative Commons Attribution 4.0 International (CC BY 4.0). See `LICENSE-CC-BY-4.0`.

## Repository version

This repository corresponds to the materials submitted with the dissertation.  
Readers are encouraged to refer to the tagged release **v1.0.0** for a stable snapshot.

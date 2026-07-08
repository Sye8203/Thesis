# Bayesian Latent Confounder Modeling of Urbanicity and Urinary Iodine Status in the Philippines

This repository contains the analysis code and data used in the undergraduate thesis:

**"Bayesian Latent Confounder Modeling of Urbanicity and Urinary Iodine Status in the Philippines"**
Syrelle Kaye D. Valiao
Bachelor of Science in Statistics, MSU-Iligan Institute of Technology
July 2026

For full results, discussion, and interpretation, please refer to the complete thesis document.

## Purpose

This repository is provided for **reproducibility**. It contains the R Markdown scripts and datasets needed to reproduce the exploratory data analysis, modeling, and sensitivity analysis presented in the study.

## Repository Structure

```
BLCM/
├── CEVAE.Rmd                  # Causal effect variational autoencoder model
├── INLA.Rmd                   # Integrated Nested Laplace Approximation model
├── data_prep.Rmd              # Data cleaning and preparation
├── eda_1.Rmd                  # Exploratory data analysis
├── sensitivity_analysis.Rmd   # Sensitivity analysis
│
├── 2025-09-05142333_biochemical/
│   ├── 2025-09-05142333_data-set_biochemical.csv
│   └── 2025-09-05142333_data-dictionary_biochemical.csv
│
├── 2025-11-18072406_socio/
│   ├── 2025-11-18072406_data-set_socio.csv
│   └── 2025-11-18072406_data-dictionary_socio.csv
│
├── 2018-19-21_Metadata_Documentation_BIOCHEM.pdf
├── 2018-19-21_Metadata_Documentation_SES_INDIV.pdf
│
└── README.md
```

## How to Reproduce

1. Clone this repository:
   ```bash
   git clone https://github.com/Sye8203/Thesis.git
   ```
2. Open the project in RStudio.
3. Run the R Markdown files in the following order:
   1. `data_prep.Rmd` — cleans and prepares the raw datasets
   2. `eda_1.Rmd` — exploratory data analysis
   3. `CEVAE.Rmd` — individual treatment modeling
   4. `INLA.Rmd` — regional level treatment modeling (main modeling)
   5. `sensitivity_analysis.Rmd` — sensitivity checks

## Data Sources

- **Biochemical and socio-economic datasets**: (ENNS data 2018-2021) [e-nutrition](https://enutrition.fnri.dost.gov.ph/)
- **Administrative boundary shapefiles** (PSA-NAMRIA, November 2023): Not included in this repository due to file size. Download directly from [PhilGIS](https://philgis.org) or the [PSA/NAMRIA source link].

## Notes

- Data dictionaries (`data-dictionary_*.csv`) describe variable names and coding schemes for each dataset.
- Metadata documentation PDFs provide additional context on how the biochemical and socio-economic data were collected.

## Citation

If you use this code or data, please cite the thesis:

> Valiao, S. K. D. (2026). *Bayesian latent confounder modeling of urbanicity and urinary iodine status in the Philippines* [Undergraduate thesis]. MSU-Iligan Institute of Technology.

## Contact

For questions about this repository, please contact the author via GitHub.

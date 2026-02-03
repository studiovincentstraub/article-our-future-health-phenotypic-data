# Assessment of phenotypic data in Our Future Health 

This repository contains Jupyter notebooks used to reproduce analyses for the paper:

> **Up to five-million-person Our Future Health cohort captures UK phenomic profiles and disease patterns, compared against the general population and other cohorts**. Vincent J. Straub*, Stefania Benonisdottir, Giovanni Scotti Bentivoglio, Neil Wary, Robert Campbell, Augustine Kong, Melinda C. Mills*
> 
> *Correspondence: vincent.straub@ndph.ox.ac.uk; melinda.mills@demography.ox.ac.uk

The notebooks reproduce figures and summary analyses describing phenotypic profiles and disease patterns in the Our Future Health (OFH) cohort and comparisons with national statistics and other large population cohorts, notably UK Biobank.

## Repository contents

```
.
├── notebooks/
│   ├── calc_diag_prev_vjs.ipynb
│   ├── calc_hse_comparison_vjs.ipynb
│   ├── calc_odds_ratio_nw.ipynb
│   ├── get_canc_prev_vjs.ipynb
│   ├── get_event_cases_vjs.ipynb
│   ├── get_meds_correlates_nw.ipynb
│   ├── get_meds_prev_vjs.ipynb
│   ├── get_meds_usage_vjs.ipynb
│   ├── get_sociodemographics_vjs.ipynb
│   ├── get_top_ten_prev_vjs.ipynb
│   ├── plot_pop_pyramid_by_ethn_gsb.ipynb
│   └── plot_pop_pyramid_gsb.ipynb
├── resources/
│   └── DNAnexus-links.md
├── README.md
├── LICENSE
├── CONTRIBUTING.md
└── .github/
    └── SECURITY.md
```

All analysis code is contained in the `notebooks/` directory.  
No raw or individual-level data are included.



## Data availability and access

This study makes use of **both restricted-access and publicly available data**.

### Restricted-access data

- **Our Future Health (OFH)** participant data are available only to registered researchers who submit a successful application to the OFH Access Board.  
  Application details: https://research.ourfuturehealth.org.uk/apply-to-access-the-data/  
  **OFH study ID used in this work:** 240228.

- **UK Biobank** data are also restricted. Interested researchers must register and apply via:  
  https://www.ukbiobank.ac.uk/use-our-data/apply-for-access/  
  **UK Biobank project ID used in this work:** 59755.

This repository does **not** contain any restricted or identifiable data. Users must obtain access independently and configure data paths locally.

### Publicly available data sources

Public data used in the analyses include:

- OFH map of clinic locations: https://go.nature.com/41oKFic  
- Health Survey for England (HSE, 2021)  
- Office for National Statistics (ONS, 2021)  
- Kurki et al. (2023)  
- All of Us Research Program data snapshots: https://www.researchallofus.org/data-tools/data-snapshots/  
- Global Burden of Disease (GBD, 2021)  
- National Disease Registration Service (NDRS, 2022)

Full details of publicly available data sources used for each figure, along with de-identified processed summary-level data, are provided in the Supplementary Tables and Supplementary Information of the paper.

## Code availability and dependencies

All analyses were conducted using:

- **Python 3.9.21**  
- **R 4.0.3**

A custom Python library, **phenofhy**, was developed to process and analyse OFH phenotypic data:

- Repository: https://github.com/studiovincentstraub/phenofhy  
- `phenofhy` is open source and currently in beta.  
- It is designed to run within the OFH trusted research environment (TRE), DNAnexus, for registered researchers.

The notebooks in this repository make use of `phenofhy` alongside standard scientific Python libraries (e.g. `numpy`, `pandas`, `scipy`, `matplotlib`, `seaborn`) and, where applicable, R for plotting and supplementary analyses.

## Reproducing the analysis

### Requirements

- Python 3.9+  
- Jupyter Notebook / JupyterLab  
- Required Python packages (see `requirements.txt` or environment documentation if provided)

### Running notebooks

Notebooks are intended to be run top-to-bottom in an environment where the required data are available locally or within a secure research environment.

Interactive example:

```bash
jupyter notebook notebooks/get_sociodemographics_vjs.ipynb
```

Non-interactive (for reproducibility checks):

```bash
jupyter nbconvert --to notebook --execute   notebooks/get_sociodemographics_vjs.ipynb   --ExecutePreprocessor.timeout=600
```


## Security

If you identify a security issue or risk of unintended data disclosure, please follow the instructions in `.github/SECURITY.md`.  
Do **not** report sensitive issues via public GitHub issues.


## Citation

If you use this repository or adapt its code, please cite the associated paper and include a link to this repository. A formal citation file (`CITATION.cff`) may be added in the future.

## License

This repository is licensed under the terms specified in the `LICENSE` file.

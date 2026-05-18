# DNAnexus Learning Resources
 
A curated collection of guides, tutorials, and notebooks for researchers using the **UK Biobank Research Analysis Platform (UKB-RAP)** or the **Our Future Health Trusted Research Environment (OFH-TRE)**.
 
---
 
## Prerequisites
 
Before working with the DNAnexus platform, the following resources provide essential foundational knowledge.
 
### Bash for Bioinformatics
An introductory course covering the command-line skills needed for bioinformatic workflows on DNAnexus.
- [Bash for Bioinformatics](https://laderast.github.io/bash_for_bioinformatics/)
### Best Practices on DNAnexus
Guidance on organising projects, managing data, and writing reproducible analyses on the platform.
- [Best Practices on the DNAnexus Platform](https://laderast.github.io/best_practices_dnanexus/)
### dx Toolkit / Command Line Interface (CLI)
The `dx` CLI is the primary tool for interacting with DNAnexus programmatically. The resources below cover installation, basic usage, and the `dxdata` Python library.
- [OpenBio dx-toolkit examples](https://github.com/dnanexus/OpenBio/tree/master/dx-toolkit)
- [DNAnexus Academy: Introduction to the CLI](https://academy.dnanexus.com/command_line_interface_cli/introduction_to_cli)
- [Getting started with `dxdata` (notebook)](https://github.com/dnanexus/OpenBio/blob/master/dxdata/getting_started_with_dxdata.ipynb)
---
 
## Working with Phenotypic Data in JupyterLab
 
The resources below demonstrate how to access, explore, and export phenotypic data using Python within a JupyterLab session on DNAnexus. Resources are applicable to UKB-RAP unless otherwise noted.
 
### Loading and Exploring Phenotypic Data
 
| Notebook | Description |
|---|---|
| [Explore phenotypic tables](https://github.com/UK-Biobank/UKB-RAP-Notebooks-Access/blob/main/JupyterNotebook_Python/A101_Explore-phenotype-tables_Python.ipynb) | Browse and query available phenotype tables |
| [Explore participant data](https://github.com/UK-Biobank/UKB-RAP-Notebooks-Access/blob/main/JupyterNotebook_Python/A102_Explore-participant-data_Python.ipynb) | Inspect individual-level participant records |
| [Explore phenotypic data (OpenBio)](https://github.com/dnanexus/OpenBio/blob/master/UKB_notebooks/ukb-rap-pheno-basic.ipynb) | Basic phenotypic queries using the DNAnexus OpenBio library |
| [Export participant data](https://github.com/UK-Biobank/UKB-RAP-Notebooks-Access/blob/main/JupyterNotebook_Python/A103_Export-participant-data_Python.ipynb) | Export selected fields to file |
| [Load cohorts and analyse phenotypic data](https://github.com/dnanexus/OpenBio/blob/master/UKB_notebooks/loading_data_into_jupyterlab.ipynb) | Define cohorts and run downstream analyses in JupyterLab |
| [Identify participants with bulk files](https://github.com/UK-Biobank/UKB-RAP-Notebooks-Access/blob/main/JupyterNotebook_Python/A109_Find-participant-bulk-files.ipynb) | Link participants to associated bulk data (e.g. imaging, omics) |
 
### Phenofhy *(OFH-TRE)*
 
[Phenofhy](https://studiovincentstraub.github.io/phenofhy/) is a Python library designed for working with phenotypic data within the Our Future Health Trusted Research Environment. It provides a streamlined interface for querying and processing OFH phenotype tables in JupyterLab.
 
- [Phenofhy documentation](https://studiovincentstraub.github.io/phenofhy/)
- [Phenofhy on GitHub](https://github.com/studiovincentstraub/phenofhy)
---
 
## Working with Genotypic Data in JupyterLab
 
### Hail
 
[Hail](https://hail.is) is an open-source framework for scalable genomic data analysis. The resources below introduce Hail and demonstrate its use within DNAnexus.
 
- [DNAnexus Hail tutorial (OpenBio)](https://github.com/dnanexus/OpenBio/tree/master/hail_tutorial)
- [Hail GWAS tutorial](https://hail.is/docs/0.2/tutorials/01-genome-wide-association-study.html)
### Accessing Genotypic Data
- [UKB-RAP Genomics notebooks](https://github.com/UK-Biobank/UKB-RAP-Notebooks-Genomics) — worked examples for loading and processing UK Biobank genotype data with Hail
### Linking Genotypic and Phenotypic Data
- [UKB Community post: linking geno and pheno data](https://community.ukbiobank.ac.uk/hc/en-gb/community/posts/16019570597277-Query-of-the-week-7-About-linking-geno-and-pheno-data)
---
 
## Building Custom Apps, Applets, and Pipelines
 
DNAnexus supports the development of portable, reproducible pipelines using applets, workflows, and the Workflow Description Language (WDL).
 
### Documentation
- [DNAnexus Academy: Building Applets](https://academy.dnanexus.com/buildingapplets)
### Video Tutorials
 
| Video | Description |
|---|---|
| [Running tools available on UKB-RAP](https://www.youtube.com/watch?v=U8QZAGwnUm0&list=PLRkZ0Fz-n3Z6ku1U9V_C2bV5kqafRwrY7&index=33) | Overview of pre-installed tools and how to execute them |
| [Creating apps/workflows and bringing your own tools](https://www.youtube.com/watch?v=A_iki_50Ig0&list=PLRkZ0Fz-n3Z6ku1U9V_C2bV5kqafRwrY7&index=30) | Packaging custom tools as DNAnexus applets |
| [Introduction to WDL on UKB-RAP](https://www.youtube.com/watch?v=2X3gbS_BHiA&list=PLRkZ0Fz-n3Z6ku1U9V_C2bV5kqafRwrY7&index=30) | Writing portable workflows with WDL |
| [Advanced WDL and Docker on UKB-RAP](https://www.youtube.com/watch?v=vyzYChm0e1g&list=PLRkZ0Fz-n3Z6ku1U9V_C2bV5kqafRwrY7&index=28) | Containerising tools with Docker for use in WDL pipelines |

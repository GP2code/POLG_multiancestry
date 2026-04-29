# Multi-ancestry analysis of POLG variants in Parkinson’s disease

`GP2 ❤️ Open Science 😍`

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.19861264.svg)](https://doi.org/10.5281/zenodo.19861264)

**Last updated:** April 2026

## Summary

This is the online repository for the manuscript titled **"Multi-ancestry analysis of POLG variants in Parkinson’s disease"**.

The notebooks generated for this manuscript are deposited here in this repository. To investigate the genetic spectrum and prevalence of POLG variants in PD across diverse ancestries, we performed POLG rare variant screening, case-control analysis, segregation analysis and rare burden test.

Based on the findings, POLG variants are overall rare in PD patients but we identified rare pathogenic variants among PD cases, suggesting that POLG-related mitochondrial dysfunction may contribute to PD in isolated instances, particularly under recessive inheritance.

## Data statement
Data used in the preparation of this article were obtained from the Global Parkinson’s Genetics Program (GP2; https://gp2.org).

All GP2 data are hosted in collaboration with the Accelerating Medicines Partnership in Parkinson’s disease, and are available via application on the website (https://amp-pd.org/register-for-amp-pd). For up-to-date information on GP2 data acquisition, access, and policies, visit https://gp2.org/. Tier 1 data can be accessed by completing a form on the Accelerating Medicines Partnership in Parkinson’s Disease (AMP®-PD) website (https://amp-pd.org/register-for-amp-pd). Tier 2 data access requires approval and a Data Use Agreement signed by your institution.

In this analysis, we used GP2 Release 11 Tier 2 data ([DOI 10.5281/zenodo.17753486](https://doi.org/10.5281/zenodo.17753486))


### Helpful Links

- [GP2 Website](https://gp2.org/)
  - [GP2 Cohort Dashboard](https://gp2.org/cohort-dashboard-advanced/)
- [Introduction to GP2](https://movementdisorders.onlinelibrary.wiley.com/doi/10.1002/mds.28494)
  - [Other GP2 Manuscripts (PubMed)](https://pubmed.ncbi.nlm.nih.gov/?term=%22global+parkinson%27s+genetics+program%22)



## Repository Orientation
- The `analysis/` directory includes all analyses performed for this manuscript.

<pre> POLG_multiancestry/ 
  ├── analysis/ 
  |     ├── 00_POLG_WGS_variant_extraction.ipynb
  |     ├── 01_POLG_CES_variant_extraction.ipynb
  |     ├── 02_POLG_segregation_analysis.ipynb
  |     ├── 03_POLG_burden_analysis.ipynb
  |     └── 04_POLG_case_control_analysis.ipynb
  ├── LICENSE
  └── README.md 
</pre>

## Analysis Notebooks
### Languages: Python and bash
| Directory | Notebooks                                                                   | Description                                   | 
|-----------|-----------------------------------------------------------------------------|-----------------------------------------------| 
|`analysis/`| `00_POLG_WGS_variant_extraction.ipynb`                                      | Rare variant extraction of POLG from WGS      |  
|`analysis/`| `01_POLG_CES_variant_extraction.ipynb`                                      | Rare variant extraction of POLG from CES      |  
|`analysis/`| `02_POLG_segregation_analysis.ipynb`                                        | Segregation analysis                          |              
|`analysis/`| `03_POLG_burden_analysis.ipynb`                                             | Burden analysis                               |              
|`analysis/`| `04_POLG_case_control_analysis.ipynb`                                       | Case-control analysis                         | 


## Software
| **Software**   | **Version(s)** | **Resource URL**                              | **RRID**        | **Notes**                                               |
|----------------|----------------|-----------------------------------------------|-----------------|---------------------------------------------------------|
|ANNOVAR         |d.06.08.2020    |http://www.openbioinformatics.org/annovar/     |RRID:SCR_012821  |Used for variant annotation.                             |
|BCFtools        |v.1.17+         |http://samtools.sourceforge.net/mpileup.shtml  |RRID:SCR_005227  |Used for genomic file manipulation.                      |
|GenoTools       |v.1.2.3         |https://github.com/GP2code/GenoTools           |NA               |Used for quality control and genetic ancestry inferrence.|
|gnomAD          |v.4.1           |http://gnomad.broadinstitute.org/              |RRID:SCR_014964  |Used to retrieve population frequency data.              |
|PLINK           |v.1.9, v.2.0    |http://www.nitrc.org/projects/plink            |RRID:SCR_001757  |Used for genetic analyses.                               |

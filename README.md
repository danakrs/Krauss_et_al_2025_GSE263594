# Bulk RNA-Seq Analysis – Krauß et al. (2025)

This repository contains the analysis workflow for [GSE263594](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE263594) bulk RNA-seq dataset as published in:
[**Krauß et al. (2025), EMBO Molecular Medicine**](https://doi.org/10.1038/s44321-025-00240-4)

DOI: 10.1038/s44321-025-00240-4


[Full rendered report](https://htmlpreview.github.io/?https://github.com/danakrs/Krauss_et_al_2025_GSE263594/blob/main/scripts/01-RNASeq_Krauss_etal_2025.html)


---

## Overview

This project reproduces the differential gene expression and downstream analyses performed in the study, including:

* Differential expression analysis using DESeq2
* Exploratory data analysis (PCA, clustering)
* Gene set enrichment analysis (GSEA)
* Pathway activity inference (PROGENy)
* Visualization (heatmaps, volcano plots, etc.)


---

## Data Availability

Sequencing data is publicly available via GEO:

* Accession: GSE263594
* Data availability from [GEO](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE263594)


---

## Experimental Design


### Sample Groups

* **AKP**: KRASG12D, P53, APC, EGFRwt
* **AKPE**: KRASG12D, P53, APC, EGFRdelta
* **AP**: KRASwt, P53, APC EGFRwt


---

## RNA-Seq Processing

* Sequencing platform: Illumina NovaSeq 6000
* Alignment: STAR (v2.6.1d)
* Quantification: Salmon (v1.4.0)
* Reference genome: GRCm38/mm10 (GENCODE M25)

Downstream analysis performed in R (4.5.1).
Package Version Information in the rendered .html file.
---



---

## Project Structure

```
├── scripts/         # analysis scripts
├── data/            # (ignored) downloaded data
├── results/         # (ignored) output tables
├── plots/           # (ignored) figures
├── README.md
├── .gitignore
```

---



---

## ⚠ Notes

* Some package versions (e.g. msigdbr) may need to match the indicated version to reproduce figures in the publication
* KEGG gene sets require older versions due to licensing changes

---



# SPatacseq  <img src="https://raw.githubusercontent.com/systemPipeR/systemPipeR.github.io/main/static/images/SPR-Workflows.png" align="right" height="139" />

<!-- badges: start -->
![R-CMD-check](https://github.com/systemPipeR/SPatacseq/workflows/R-CMD-check/badge.svg)
[![Lifecycle: experimental](https://img.shields.io/badge/lifecycle-experimental-orange.svg)](https://www.tidyverse.org/lifecycle/#experimental)
[![Project Status: Active – The project has reached a stable, usable state and is being actively developed.](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active)
<!-- badges: end -->

### :construction: Under Development!

> This pipeline is currently under development and does not have a stable release yet.

### Installation

To install the package, please use the _`BiocManager::install`_ command:
```
if (!requireNamespace("BiocManager", quietly=TRUE))
    install.packages("BiocManager")
BiocManager::install("systemPipeR/SPatacseq", build_vignettes=TRUE, dependencies=TRUE)
```
To obtain the *systemPipeR* and *systemPipeRdata*, please run as follow:
```
if (!requireNamespace("BiocManager", quietly=TRUE))
    install.packages("BiocManager")
BiocManager::install("systemPipeR")
BiocManager::install("systemPipeRdata")
```
### Usage

### Pipeline summary

- Read Preprocessing
  - Preprocessing with _`preprocessReads`_ function
  - Preprocessing with TrimGalore!
  - Preprocessing with Trimmomatic
- FASTQ quality report
- Alignment against reference genome
    - Alignment with _`Bowtie2`_ 
    - Alignment with _`BWA`_ 
- Create symbolic links for viewing BAM files in IGV
- Peak calling with MACS2
- Annotate peaks 
    - Annotation with `ChIPpeakAnno` package
    - Annotation with `ChIPseeker` package
- Count reads overlapping peaks
- Differential binding analysis
- GO term enrichment analysis
- Motif analysis
    - Motif discovery with `BCRANK`
# SPatacseq

<!-- badges: start -->
![R-CMD-check](https://github.com/systemPipeR/SPatacseq/workflows/R-CMD-check/badge.svg)
[![Lifecycle: experimental](https://img.shields.io/badge/lifecycle-experimental-orange.svg)](https://www.tidyverse.org/lifecycle/#experimental)
[![Project Status: Active – The project has reached a stable, usable state and is being actively developed.](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active)
<!-- badges: end -->

### Introduction

### Installation
```r
if (!requireNamespace("BiocManager", quietly = TRUE)) {
  install.packages("BiocManager") }
BiocManager::install("systemPipeR/SPatacseq"")
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
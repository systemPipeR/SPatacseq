# SPatacseq <img src="https://raw.githubusercontent.com/systemPipeR/systemPipeR.github.io/main/static/images/SPR-Workflows.png" align="right" height="139" />

<!-- badges: start -->
[![R-CMD-check](https://github.com/systemPipeR/SPatacseq/actions/workflows/R_CMD.yml/badge.svg)](https://github.com/systemPipeR/SPatacseq/actions/workflows/R_CMD.yml)
[![Lifecycle: experimental](https://img.shields.io/badge/lifecycle-experimental-orange.svg)](https://www.tidyverse.org/lifecycle/#experimental)
[![Project Status: Active – The project has reached a stable, usable state and is being actively developed.](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active)
<!-- badges: end -->

### :construction: Under Development!

> This pipeline is currently under development and does not have a stable release yet.

### Installation

To obtain the *systemPipeR* and *systemPipeRdata*, please run as follow:
```
if (!requireNamespace("BiocManager", quietly=TRUE))
    install.packages("BiocManager")
BiocManager::install("systemPipeR")
BiocManager::install("systemPipeRdata")
```

### Usage

To test workflows quickly or design new ones from existing templates, users can
generate with a single command workflow instances fully populated with sample data 
and parameter files required for running a chosen workflow.

Use `git` or `git-bash.exe` (Windows) to download the template and run 

```
git clone https://github.com/systemPipeR/SPatacseq.git
cd SPatacseq
```

To init the workflow management instance, run
```r
library("systemPipeR")
sal <- SPRproject()
sal <- importWF(sal, file_path = "SPatacseq.Rmd")
```

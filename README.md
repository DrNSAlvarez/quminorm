# Quantile normalization of single-cell RNA-seq read counts without unique molecular identifiers

<!-- badges: start -->
  [![Travis build status](https://travis-ci.com/willtownes/quminorm.svg?branch=master)](https://travis-ci.com/willtownes/quminorm)
  [![codecov](https://codecov.io/gh/willtownes/quminorm/branch/master/graph/badge.svg)](https://codecov.io/gh/willtownes/quminorm)
<!-- badges: end -->

## About

The purpose of this package is to remove PCR distortion from scRNA-seq read counts by normalizing to quasi-UMI counts (QUMIs). QUMIs approximate the true (unmeasured) UMI counts. Once read counts or TPM are transformed to QUMIs, the count matrix can be passed to UMI-specific methods for feature selection and dimension reduction, such as those provided in the [scry package](https://bioconductor.org/packages/release/bioc/html/scry.html).

For more details see the [Genome Biology paper](https://doi.org/10.1186/s13059-020-02078-0). Please cite the publication if you use this package in your research. If you find bugs please create a [github issue](https://github.com/willtownes/quminorm-paper/issues).

See the DESCRIPTION file for a list of authors and contributors.

## Installation via conda
```{r}
Fork willtownes/quminorm to <your_account>
git clone https://github.com/<your_account>/quminorm
cd quminorm/
git tag v1.0.0
git push --tags
conda skeleton cran https://github.com/<your_account>/quminorm
conda build --R=4.1.0 r-quminorm
```
## Usage

Please refer to the vignettes.

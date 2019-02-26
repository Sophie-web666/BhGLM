# BhGLM: Bayesian hierarchical GLMs and survival models, with applications to Genomics and Epidemiology 

# Overview

This R package provides functions for setting up and fitting various Bayesian hierarchical models (generalized linear models (GLMs), Cox survival models, negative binomial models, and ordered logistic or probit regressions), for numerically and graphically summarizing the fitted models, and for evaluating the predictive performance. Several types of priors on the coefficients can be used: double-exponential, Student-t, mixture double-exponential, and mixture t. The models are fitted by using fast algorithms for estimating posterior modes rather than MCMC. The methods can be used to analyze not only general data but also large-scale molecular data (i.e., detecting disease-associated genes or variants, predictive and prognostic modeling of diseases and traits, etc).

(note: the function glmm.nb for negative binomial mixed models has been moved to the package NBZIMM http://github.com//nyiuab//NBZIMM). 

Author: Nengjun Yi <nyi@uab.edu>;  Maintainer: Nengjun Yi <nyi@uab.edu>

# Installation

Three ways to install the package in R:

1. Without Vignettes
```{r}
if (!requireNamespace("devtools")) install.packages("devtools")
library(devtools)
install_github("nyiuab/BhGLM")
```
2. With Vignettes
```{r}
if (!requireNamespace("devtools")) install.packages("devtools")
library(devtools)
install_github("nyiuab/BhGLM", build_opts = c("--no-resave-data", "--no-manual"), force = T)
```
3. Download the BhGLM zip file to your computer, and then install it to R.

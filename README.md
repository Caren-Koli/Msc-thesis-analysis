
# MSc Thesis Analysis

This repository contains the R code used for my MSc dissertation analysis titled:

**A comparative evaluation of Bayesian logistic and frequentist logistic regression models in estimating risk of hypertension: Application to multilevel STEPs survey data**

The analysis uses the 2015 Kenya WHO STEPs survey data to estimate risk factors for hypertension while accounting for the complex survey design, clustering, and potential outcome misclassification.

The main analysis focuses on estimating **marginal population-averaged risk ratios** for hypertension using g-computation. Conditional odds ratios, intraclass correlation coefficients, and variance components from multilevel models are reported as supporting analyses to assess clustering and contextual variation.

## Analytical workflow

The code follows the main thesis workflow:

1. Data cleaning and preparation of the Kenya STEPs analytical dataset.
2. Description of the survey structure, missing data, sampling weights, effective sample size, and design effects.
3. Estimation of hypertension prevalence using the WHO STEPs composite definition.
4. Fitting of frequentist two-level logistic models using `svyglm` and `lme4`.
5. Fitting of Bayesian two-level logistic models using pseudo-posterior weighting.
6. Estimation of marginal risk ratios using model-based predicted probabilities and g-computation.
7. Supporting sensitivity analyses, including alternative hypertension definitions, probabilistic bias analysis, and three-level model checks.
8. Model evaluation using predictive metrics: LOO-CV, ELPD, calibration, Brier score, and cross-validation.

## Repository contents

* `script.Rmd`: Main reproducible R Markdown script containing the thesis analysis code.
* `Analysis.Rproj`: RStudio project file for running the analysis in a consistent project environment.
* `README.md`: Description of the repository and analytical workflow.
* `.gitignore`: Files and folders excluded from version control.

## Notes

The raw STEPs survey dataset is not included in this repository because of data access restrictions. The code is provided for transparency and reproducibility of the analytical workflow used in the thesis.

## License
This repository is provided for academic transparency and reproducibility of the thesis analysis. The R code may be reused or adapted for academic and non-commercial purposes with appropriate acknowledgement.

## Author
Caren Koli,
Strathmore University,
June 2026

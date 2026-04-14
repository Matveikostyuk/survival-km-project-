# Survival Analysis in R: Kaplan–Meier & Cox Regression

## Overview
This project demonstrates a full survival analysis workflow applied to clinical lung cancer data using R. The analysis includes Kaplan–Meier survival estimation, group comparison using the log-rank test, and multivariable modeling with Cox proportional hazards regression.

The goal of this project is to showcase applied biostatistics skills relevant to clinical and translational research, particularly in oncology.

---

## Dataset
The analysis uses the built-in `lung` dataset from the `survival` R package. This dataset contains clinical and survival information for patients with advanced lung cancer.

Key variables include:
- Survival time (days)
- Event status (death vs censored)
- Age
- Sex
- ECOG performance status

---

## Methods

### 1. Data preprocessing
- Removal of missing values
- Conversion of survival status into a binary event indicator (1 = death, 0 = censored)

### 2. Kaplan–Meier survival analysis
- Estimation of overall survival probability
- Visualization of survival curves with confidence intervals
- Inclusion of risk tables

### 3. Stratified survival analysis
- Comparison of survival between male and female patients
- Visualization of group-specific survival curves

### 4. Log-rank test
- Statistical comparison of survival distributions between groups

### 5. Cox proportional hazards model
- Multivariable analysis including:
  - Age
  - Sex
  - ECOG performance status
- Estimation of hazard ratios (HR) and confidence intervals

---

## Results Summary
- Kaplan–Meier curves demonstrate the decline in survival probability over time
- Differences in survival between sex groups are assessed using the log-rank test
- Cox regression identifies clinical variables associated with increased hazard of death
- Findings are consistent with known prognostic factors in oncology

---

## Output
- Kaplan–Meier survival plots (overall and stratified)
- Log-rank test results
- Cox model summary (hazard ratios, p-values)
- Exported survival plot: `km_sex_plot.png`

---

## Tools and Technologies
- R
- survival package
- survminer package

---

## Reproducibility
The analysis is fully reproducible using the provided R script:

```r
source("km_analysis.R")

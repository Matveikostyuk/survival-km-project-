# Survival Analysis in R: Kaplan–Meier & Cox Regression

## Overview
This project demonstrates a survival analysis workflow applied to clinical lung cancer data using R. The analysis includes Kaplan–Meier survival estimation, log-rank testing, and Cox proportional hazards modeling.

This project is designed to showcase applied biostatistics skills relevant to oncology and translational research.

---

## Dataset
The analysis uses the built-in `lung` dataset from the `survival` package, which contains clinical and survival data for patients with lung cancer.

---

## Methods
- Kaplan–Meier survival analysis
- Group comparison by sex
- Log-rank test
- Cox proportional hazards model

---

## Results

Kaplan–Meier analysis demonstrated a difference in survival between male and female patients, with females showing improved survival probability over time.

The log-rank test indicated that this difference was statistically significant (p = 0.014).

In the Cox proportional hazards model, increasing age and worse ECOG performance status were associated with higher hazard of death, consistent with established clinical prognostic factors.

---

---

## Tools
- R
- survival
- survminer

---


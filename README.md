# Asthma Risk Analysis (R)

This project explores environmental and demographic factors influencing asthma cases using statistical and machine learning models in R.  
It demonstrates a full end-to-end data science workflow — from data cleaning and exploration to predictive modelling and interpretation.

---

## Overview

**Objective:**  
Identify key environmental variables associated with asthma prevalence and develop models to predict the likelihood of asthma cases.

**Dataset:**  
Simulated environmental and demographic data including:
- Air pollutants (CO, NO₂, O₃, SO₂, PM10)
- Weather metrics (precipitation, humidity, windspeed)
- Demographic factors (age group, gender, postcode)

---

## Methods

| Step | Technique | Purpose |
|------|------------|----------|
| 1 | **Data Cleaning & Exploration** | Prepare and visualise trends across pollutants, humidity, and asthma rates |
| 2 | **Logistic Regression** | Build baseline predictive models and evaluate key drivers |
| 3 | **Polynomial Logistic Regression** | Capture potential nonlinear effects in environmental factors |
| 4 | **Decision Tree Modelling** | Identify clear, interpretable rules for asthma risk profiles |
| 5 | **Unsupervised Learning (Clustering)** | Detect hidden patterns among environmental conditions |
| 6 | **Model Evaluation** | Compare accuracy, interpretability, and generalisation performance |

---

## Final Logistic Regression Model

\[
\text{logit}(p) = -1.358 + 0.012(\text{NO₂}) + 2.103(\text{CO}) - 0.026(\text{O₃}) + 0.879(\text{Precipitation}) + 0.009(\text{Relative Humidity})
\]

- **Accuracy:** 71.9% (on test data)  
- **Interpretation:** Asthma likelihood increases with higher CO and rainfall, and decreases with higher O₃ levels.

---

## Decision Tree Summary

- **Key splits:** O₃, Vapour Pressure, and Precipitation  
- **Accuracy (pruned tree):** 70%  
- **Interpretation:**  
  - Low O₃ (<12.5) + low vapour pressure → high asthma risk  
  - Higher O₃ and lower precipitation → lower risk group

---

## Tools & Libraries

- **Language:** R  
- **Libraries:** `tidyverse`, `ISLR`, `tree`, `e1071`, `caret`  
- **Environment:** RStudio / Jupyter (R kernel)

---

## Folder Structure


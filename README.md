# Statistical Machine Learning Final Project — Spring 2026

## Overview
This project analyzes and predicts violent crime rates across U.S. communities using socioeconomic and demographic data. We evaluate multiple statistical and machine learning models to understand which approaches best capture the underlying relationships in the data.

The focus is on comparing **regularized linear models, distance-based methods, and dimension reduction techniques** in a high-dimensional setting.

---
### Data Source 
The data for this project was provided by the UCI Machine Learning Repository. It is a culmination of three socio-economic datasets on communities within the United States: 
-  1990 US Census
-  1990 US LEMAS 
    - Only police deparments with at least 100 officers were used, plus a random sample of smaller deparments. 
-  1995 FBI UCR

https://archive.ics.uci.edu/dataset/183/communities+and+crime

### Target Variable
- `ViolentCrimesPerPop` — normalized measure of violent crime rate

---

### Models Used

We implemented and compared the following models:

- LASSO Regression
- Ridge Regression
- K-Nearest Neighbors (KNN)
- Principal Component Regression (PCR)
- Partial Least Squares (PLS)

---

## Results Summary

| Model  | RMSE | R²   | Tuning Parameter |
|--------|------|------|------|
| LASSO  | 0.136 | 0.648 | Alpha = 0.0007 |
| Ridge  | 0.138 | 0.688 | Alpha = 138.489 |
| KNN    | 0.147 | 0.590 | k = 15 | 
| PCR    | 0.142  | 0.620 | Components = 34 |
| PLS    | 0.137  | 0.645 | Components = 15 |

---

## Contributions

| Team Member       | Contributions |
|------------------|-------------|
| Alexis Seidle     |KNN, PowerPoint Presentation |
| Joe Ledford           | Data Preprocessing, LASSO, PLS |
| Sarah Fischer           | Ridge Regression, PCR |


---

### Sources
Redmond, M. (2002). Communities and Crime [Dataset]. UCI Machine Learning Repository. https://doi.org/10.24432/C53W3X. 

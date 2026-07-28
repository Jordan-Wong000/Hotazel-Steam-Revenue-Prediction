```markdown
# Hotazel Steam: Revenue Forecasting Analysis

## Overview
This notebook presents an analysis of revenue forecasting for Hotazel Steam using linear regression models. The primary goal is to predict revenue based on production figures, incorporating seasonal effects through dummy variables and interaction terms. Two models are developed and compared to identify the most accurate forecasting approach.

## Models Developed

### Model 1: Winter Season Impact
*   **Objective:** To assess the impact of winter months (December, January, February) on revenue.
*   **Variables:** `production`, `winter_DV` (dummy variable for winter months), and `winter_interaction` (`production` * `winter_DV`).
*   **Methodology:** An OLS regression model (`model1`) was trained on `dt4training` data.
*   **Performance:** Achieved a Mean Absolute Percentage Error (MAPE) of **15.9%** on the `dt4testing` dataset.

### Model 2: Summer Season Impact
*   **Objective:** To assess the impact of summer months (June, July, August) on revenue.
*   **Variables:** `production`, `summer_DV` (dummy variable for summer months), and `summer_interaction` (`production` * `summer_DV`).
*   **Methodology:** An OLS regression model (`model2`) was trained on `dt4training2` data.
*   **Performance:** Achieved a Mean Absolute Percentage Error (MAPE) of **19.7%** on the `dt4testing2` dataset.

## Conclusion and Recommendation
Based on the Mean Absolute Percentage Error (MAPE) scores, **Model 1 (Winter Season Impact)** significantly outperformed Model 2, yielding a lower MAPE of 15.9% compared to Model 2's 19.7%. This indicates that Model 1 provides more accurate predictions on unseen data.

**Recommendation:** Model 1 is recommended for forecasting Hotazel Steam's revenue, as it demonstrates superior predictive performance and better captures the underlying patterns in the data.

## Resources
*   `AICPA_regressionAnalysisData.csv`: The dataset used for training and testing the models.
```

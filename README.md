```markdown
# README: ML-Based Imputation of Missing Nutrition Data in Humanitarian Surveys

This notebook replicates the analysis presented in the paper:
>*'Machine Learning-Based Imputation of Missing Household Nutrition Data in Humanitarian Surveys: A Comparative Study Using DHS-Consistent Data from Northeast Nigeria'* by Joshua Samuel Dauda.

## Overview

This study compares various machine learning-based imputation methods for handling missing 'Weight-for-Height Z-score' (WHZ) data, a proxy for acute malnutrition, in humanitarian surveys. The dataset used is a simulated DHS-consistent dataset reflecting the demographic and nutritional structure of Northeast Nigeria.

## Key Sections:

1.  **Environment Setup**: Imports necessary libraries and sets up the environment.
2.  **Data Generation**: Simulates a DHS-consistent child nutrition dataset.
3.  **Introduce Missing Data**: Artificially introduces missing data into the 'whz' variable using three mechanisms: Missing Completely At Random (MCAR), Missing At Random (MAR), and Missing Not At Random (MNAR).
4.  **Visualize Missing Patterns**: Illustrates the introduced missing data patterns, particularly by wealth quintile.
5.  **Evaluation Function**: Defines functions for setting up different imputers (Mean, KNN, MICE, Random Forest) and evaluating their performance based on RMSE, MAE, R², and Bias.
6.  **Run Comparison**: Executes the imputation methods across all three missing data mechanisms and presents the results.
7.  **Figure 2 — RMSE Comparison Bar Chart**: Visualizes the RMSE performance of each imputation method for different missingness mechanisms.
8.  **Figure 3 — Scatter: True vs Imputed WHZ (MAR)**: Compares true WHZ values with imputed values for Mean and Random Forest imputation under the MAR mechanism.
9.  **Figure 4 — GAM Prevalence Estimation Error**: Assesses how accurately each method estimates the prevalence of Global Acute Malnutrition (GAM).
10. **Sensitivity Analysis — Varying Missingness Rate**: Examines the RMSE performance of imputers as the missingness rate increases under the MAR mechanism.
11. **Figure 6 — Feature Importance**: Shows the feature importance for WHZ prediction using a Random Forest Regressor.

This notebook provides a comprehensive comparison and visualization of different imputation techniques for a critical public health variable.
```
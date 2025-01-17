# Table of Contents
 - [Executive Summary](#executive-summary)
 - [Key Findings](#key-findings)
 - [Introduction](#introduction)
 - [Dataset Overview](#dataset)
 - [Methodology](#methodology)
   - [Regression Models](#regression-models)
 - [Results](#results)
 - [Dashboard](#dashboard-material)


# Executive Summary

This project aimed to create a machine learning regression model to predict house prices accurately and develop an interactive Tableau dashboard for stakeholders to explore and visualize house price data. The final model achieved an R² Test Score of 0.87, indicating strong predictive performance, and the dashboard provides a user-friendly platform for exploring trends and patterns.

# Key Findings
  - Model Performance: The XGBoost model with parameters (learning_rate=0.1, max_depth=5, n_estimators=300) outperformed other models, achieving an R² Test Score of 0.87 and a Root Mean Squared Error (RMSE) of approximately 81,952.
  - Feature Insights: Key features affecting house prices included location, square footage, and year built.
  - Stakeholder Accessibility: The Tableau dashboard enables stakeholders to interactively visualize house prices, explore relationships between features, and identify trends.
<img width="687" alt="Screenshot 2024-08-13 at 22 00 28 copy" src="https://github.com/user-attachments/assets/925e302b-af37-4ec2-9ee7-c19e82811075">

# Introduction

The goal of this project was twofold:
	1.	Develop a robust machine learning model to predict house prices accurately.
	2.	Create an interactive dashboard to enable stakeholders to visualize and explore house price data effectively.

# Dataset 
 - **Source:** Dataset linked here: Full Dataset Link | Cleaned Dataset Link
 - **Size:** 21,060 entries with 15 features.
 - **Memory Usage:** 2.4+ MB.
 - **Features:** Include price, location, square footage, number of bedrooms, and year built.

# Methodology
 - **Data Preparation:** Cleaned the dataset, performed feature engineering, and handled missing values.
 - **Model Selection:** Evaluated multiple regression models before applying grid search to optimize the XGBoost model for the best performance.
   - Linear Regression
   - Polynomial Regression
   - Ridge Regression
   - Lasso Regression
   - Elastic Net
   - XGBoost
- **Visualization:** Built an interactive Tableau dashboard to present findings and enable data exploration.

### Regression Models
 - **Linear Regression:** Established baseline performance.
 - **Polynomial Regression:** Improved accuracy but prone to overfitting.
 - **Ridge and Lasso:** Improved regularization but underperformed compared to XGBoost.
 - **Elastic Net:** Balanced regularization approach but not as effective as XGBoost.
 - **XGBoost:** Final model selected due to superior performance.

# Results
| Metric | Value |
| --- | --- |
| R² Test Score | 0.87 |
| R² Train Score | 0.91 |
| Test Root Mean Squared Error | 81951.69 |
| Train Root Mean Squared Error | 71595.41 |
| Mean Absolute Error | 6716080061.49 |

# Dashboard Material

### [Tableau Link](https://public.tableau.com/views/P1_House_Price_Prediction_Dashboard/Seattle?:language=en-GB&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)

<img width="1512" alt="Dashboard" src="https://github.com/user-attachments/assets/d57a097d-0ef3-4280-85eb-d118ee8563cc">

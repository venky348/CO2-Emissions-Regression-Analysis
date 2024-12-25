# CO2 Emissions Regression Analysis

This project focuses on a **regression machine learning problem** to analyze vehicle-related CO2 emissions. Using a dataset of 7,385 entries and 12 attributes, it explores the relationships between vehicle features and their environmental impact, employing data preprocessing, exploratory data analysis (EDA), and various regression models.

---

## Overview

This repository examines CO2 emissions and their relationships with vehicle attributes such as:
- Engine size
- Fuel consumption
- Transmission type
- Vehicle class
- Fuel type

The project employs:
- **Exploratory Data Analysis (EDA)** for insights into relationships and distributions.
- **Correlation Analysis** to understand the strength of relationships.
- **Regression Models** (Linear, Ridge, Lasso, ElasticNet) to predict CO2 emissions.

---

## Dataset Details

- **Entries:** 7,385
- **Attributes:** 12 (7 continuous, 5 categorical)
- **Key Features:**
  - Continuous: Engine size, fuel consumption metrics, CO2 emissions.
  - Categorical: Make, model, transmission, fuel type, vehicle class.

---

## Key Insights

### 1. Exploratory Data Analysis (EDA)
- **Positive Correlations:** Higher engine size and fuel consumption increase CO2 emissions.
- **Negative Correlation:** Fuel efficiency (mpg) inversely impacts CO2 emissions.
- **Outliers:** Certain vehicles with unusual emissions and consumption patterns were identified for further investigation.

### 2. Machine Learning Models
#### Linear Regression
- Achieved competitive performance with a cross-validation MSE of 318.50.

#### Ridge Regression
- Best performance with α=0.1:
  - Train MSE: 316.96
  - Test MSE: 329.58

#### Lasso Regression
- Best results at α=0.01:
  - Test MSE: 329.62

#### ElasticNet
- Best results with α=0.001 and l1_ratio=0.5:
  - Test MSE: 329.67

---

## Results Summary

- **Higher fuel consumption leads to higher emissions.**
- **Ridge and Lasso models performed consistently better than others.**
- **Improving fuel efficiency significantly reduces environmental impact.**

---


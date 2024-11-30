# Maternal-Health-Risk-Analysis

## Table of Contents
- [Overview](#overview)
- [Data Sources](#data-sources)
- [Data cleaning and preprocessing](#data-cleaning-and-preprocessing)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Technologies used](#technologies-used)
- [Data Analysis](#data-analysis)
- [Features](#features)
- [Visualization](#visualization)
- [Findings](#findings)
- [Recommendations](#recommendations)


## Overview

The basis of analyzing maternal health data is to identify key risk factors contributing to high maternal mortality rates, focusing on: factors associated with maternal health risk level and What interventions can reduce maternal mortality rates

The goal is to provide actionable insights to inform healthcare interventions and policies.

This project analyzes the correlation between different health indicators that play a crucial role in determining maternal health risk using statistical methods and data visualization techniques.

## Data Sources

Data has been collected from different hospitals, community clinics, maternal health cares from the rural areas of Bangladesh through the IoT based risk monitoring system.

## Data cleaning and preprocessing

In the initial data preprosseing we perform the following tasks:
- Data loading and inspection.
- Handling missing values.
- Data cleaning and formatting

## Exploratory Data Analysis

EDA involves exploring the maternal health risk data and answer the following questions:
- Correlation between risk factors and health risk level
- Risk Distribution by Age Group.
- Relationship between (SystolicBP) and Risk Level

## Technologies used

- Python: For data manipulation and analysis.

- Pandas:For handling and cleaning data.

- Matplotlib and Seaborn: For data visualization.
- Power Point: For report writing.

## Data Analysis

```python
#EDA
#Which variables are most strongly correlated with RiskLevel?
# Convert Categorical column 'RiskLevel' to numerical for analysis
data['RiskLevel'] = data['RiskLevel'].map({'low risk': 0, 'mid risk': 1, 'high risk': 2})

correlation = data.corr()
print("Correlation Matrix:\n", correlation)
```

## Features
- Heatmap to analyze the correlation between risk factors and health risk level.
- Bar chart of risk distribution by Age Group.
- Box plot of the relationship between (SystolicBP) and Risk Level

## Visualization

Heatmap to analyze the correlation between risk factors and health risk level.

![Heat map](https://github.com/user-attachments/assets/fe84d8d0-f8a0-4dac-875d-64541fdabd93)


Bar chart of risk distribution by Age Group.

![Bar chart](https://github.com/user-attachments/assets/ae26ba72-fdf0-4d62-bc98-c0b987c35740)


Box plot of the relationship between (SystolicBP) and Risk Level


![Box plot](https://github.com/user-attachments/assets/1ac12892-05be-420b-ae1c-d418ecba9ec8)


## Findings
- There is a strong correlation between key factors (e.g., blood sugar, systolic BP) and maternal risk levels.
- Certain age groups show a higher likelihood of being classified under high-risk levels.
- High systolic readings are common in high-risk cases.
- High blood sugar levels are more prevalent in higher maternal risk categories

## Recommendations
- Develop targeted health screening programs focusing on high-risk Age groups and physiological profiles.
- Focused monitoring of high-risk individuals using key health indicators




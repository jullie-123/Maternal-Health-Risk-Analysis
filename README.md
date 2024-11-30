# Maternal-Health-Risk-Analysis

## Table of Contents
- [Overview](#overview)
- [Data Sources](#data-sources)
- [Data cleaning and preprocessing](#data-cleaning-and-preprocessing)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Technologies used](#technologies-used)
- [Data Analysis](#data-analysis)
- [Features](#features)


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








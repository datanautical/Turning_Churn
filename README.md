# Telco Customer Churn Analysis
### Statistical Evidence of Contract Impact on Customer Retention

---

## Overview

This project analyzes customer churn behavior in a telecommunications dataset to identify the factors most strongly associated with customer attrition.

Developed as part of a formal data analytics thesis, this work demonstrates the application of statistical methodology to a real-world telecommunications problem. The focus is on clear, reproducible analysis rather than black-box modeling, emphasizing foundational data science principles that produce trustworthy business insight.

At the center of this analysis is a critical business question:

> **Does contract type significantly influence customer churn?**

Rather than jumping directly into machine learning, this project emphasizes **statistical rigor, reproducibility, and clear interpretation** of results that can be understood by both technical and non-technical stakeholders.

---

## Objective

The primary objective of this analysis is to determine whether there is a statistically significant relationship between:

- **Contract Type** (Month-to-Month, One Year, Two Year)
- **Customer Churn Status** (Yes / No)

This relationship is tested using a **Chi-Square Test of Independence** and measured for strength using **Cramér’s V** effect size.

---

## Dataset

- **Source:** IBM Telco Customer Churn sample dataset hosted on Kaggle
- **Records:** ~7,000 customers
- **Use Case:** Educational and analytical (de-identified data)

Key features include:

- Contract type
- Tenure
- Internet service
- Payment method
- Monthly charges
- Churn status

---

## Methodology

### 1. Data Cleaning & Preparation
- Handling missing values
- Data type normalization
- Construction of contingency tables

### 2. Statistical Testing
- Chi-Square Test using `scipy.stats.chi2_contingency`
- Verification of test assumptions (expected cell counts ≥ 5)
- Calculation of chi-square statistic, p-value, and degrees of freedom

### 3. Effect Size Measurement
- Cramér’s V calculation to measure practical significance

### 4. Visualization
- Bar chart comparing churn rates across contract types

### 5. Interpretation
- Clear explanation of statistical findings
- Translation of results into business implications

---

## Key Finding

The analysis reveals a **statistically significant relationship** between contract type and customer churn.

Customers on **month-to-month contracts** exhibit substantially higher churn rates compared to customers on one-year or two-year agreements. The effect size confirms this is not only statistically significant but also practically meaningful for business decision-making.

This insight provides actionable direction for customer retention strategies in telecommunications environments.

---

## Repository Structure

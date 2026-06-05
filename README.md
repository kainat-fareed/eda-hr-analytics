# Promotion Readiness Analysis – EDA Project  
### HR Analytics Case Study  

---

## Overview
Only **8.52% of employees are promoted** in this dataset — but what actually drives promotion decisions?

This project analyzes **78,298 employee records** from a multinational organization to uncover:
- Key drivers of promotions  
- Potential patterns in decision-making  
- High-performing employee signals  
- Data quality issues affecting HR analytics  

The goal is to transform raw HR data into **actionable business insights**.

---

## Business Problem
Organizations often struggle with fair and consistent promotion decisions:

- High-performing employees may be overlooked  
- Promotion patterns vary across departments and regions  
- Decisions often lack a data-driven foundation  

This project uses **exploratory data analysis (EDA)** to uncover patterns and support better HR decision-making.

---

## Dataset

- Source: Kaggle HR Analytics Dataset  
- Total records: **78,298 employees**  
- Train: 54,808 (70%)  
- Test: 23,490 (30%)  
- Both splits share identical features  

**Key Features:**
age, previous_year_rating, length_of_service, awards_won, avg_training_score

---

## What I Did

### Data Cleaning
- Handled missing values:
  - education → filled with "Unknown"  
  - previous_year_rating → filled using mode  
- Verified consistency across train/test datasets  

### Exploratory Data Analysis
- Univariate analysis of numerical & categorical variables  
- Bivariate analysis to identify promotion-related patterns  
- Correlation heatmap to check multicollinearity  

---

## Key Findings

- Promotion is highly imbalanced:
  - **8.52% promoted vs 91.48% not promoted**

- Strongest drivers of promotion:
  - previous_year_rating  
  - avg_training_score  
  - awards_won  

- Promotion patterns vary across:
  - departments  
  - education levels  
  - recruitment channels  

- Some high-performing employees appear under-promoted in specific departments  

- No significant multicollinearity → dataset is suitable for ML modeling  

---

## Technologies Used
Python, Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn

---

## Next Steps
- Feature encoding  
- Handling class imbalance  
- Model building (Logistic Regression, Random Forest, XGBoost)  
- Model evaluation & optimization  

---

## Project Impact

- Identifies patterns in promotion decisions  
- Highlights potential fairness concerns for further investigation  
- Builds a machine-learning-ready dataset  
- Enables predictive HR analytics for decision support  

---

## Conclusion
Employee promotion decisions are largely influenced by performance metrics such as training scores, past ratings, and recognition.

This analysis demonstrates how data can be used to move from **subjective decisions → evidence-based HR strategy**.

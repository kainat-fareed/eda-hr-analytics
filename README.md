# Promotion Readiness Analysis – EDA Project  
### A Data-Driven HR Analytics Case Study | GlobeHR  

---

## Project Overview
This project analyzes a large-scale HR dataset from a multinational organization (GlobeHR) operating across 28 regions with over 78,298 employees.

The objective is to explore promotion patterns, identify key performance drivers, uncover potential biases, and prepare the dataset for machine learning modeling.

This repository includes a complete Exploratory Data Analysis (EDA) pipeline, data cleaning workflow, visualizations, and actionable insights.

---

## Business Problem
Every year, GlobeHR conducts an internal promotion cycle. However, several challenges were identified:

- Only ~8% of employees are promoted  
- High-performing employees may be overlooked  
- Promotion decisions vary across departments and regions  
- Possible bias in gender, education, and recruitment channels  
- Lack of data-driven decision-making  

This project addresses these issues using Python-based data analysis and statistical methods.

---

## Objectives
- Clean and prepare the dataset for analysis and modeling  
- Identify key drivers of employee promotion  
- Detect potential bias in HR decisions  
- Explore high-potential employees  
- Build a machine-learning-ready dataset  
- Provide actionable HR insights  

---

## Technologies Used
- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  
- Scikit-learn  

---

## Dataset Information
- Dataset contains **train (70%) and test (30%) splits**  
- Total records: 78,298 employees  
- Train: 54,808 records  
- Test: 23,490 records  
- Both datasets share identical features  

---

## 📊 Exploratory Data Analysis (EDA)

### Data Understanding
- Both train and test datasets show similar distributions across key features  
- Descriptive statistics confirm consistent behavior across datasets  
- The test dataset is representative of the training data  
- Key numerical features include:
  - age  
  - previous_year_rating  
  - length_of_service  
  - awards_won  
  - avg_training_score  

---

### Univariate Analysis
- Identified a highly imbalanced target variable (`is_promoted`)  
- Analyzed distributions of numerical and categorical variables  
- Observed variation in feature distributions across dataset  

---

### Bivariate Analysis
- Explored relationship between features and promotion status  
- Strong association found with:
  - avg_training_score  
  - previous_year_rating  
  - awards_won  
- Promotion rates vary across:
  - departments  
  - education levels  
  - recruitment channels  
- Performance and organizational factors strongly influence promotions  

---

### Multivariate Analysis
- Used correlation heatmap to analyze relationships among numerical features  
- No significant multicollinearity observed  
- Features show independent behavior suitable for modeling  

---

## Key Findings
- The dataset is highly imbalanced:
  - 8.52% employees promoted  
  - 91.48% not promoted  

- Missing values were found in:
  - education: 2,409 (train), 1,034 (test)  
  - previous_year_rating: 4,124 (train), 1,812 (test)  

- Missing values were handled as:
  - education → imputed with "Unknown"  
  - previous_year_rating → imputed using mode  

- Most important factors influencing promotion:
  - previous_year_rating  
  - avg_training_score  
  - awards_won  
  - department  
  - education  

- Statistical analysis confirmed strong relationships between promotion and key categorical variables  

---

## Conclusion
Employee promotion decisions are primarily influenced by performance-related metrics such as training scores, previous ratings, and recognition. Organizational factors like department and education also play an important role.

The dataset is well-structured and suitable for building predictive machine learning models.

---

## Next Steps
- Feature encoding  
- Handling class imbalance  
- Model building (Logistic Regression, Random Forest, XGBoost)  
- Model evaluation and optimization  

---

## Project Impact
- Identifies bias in promotion decisions  
- Highlights overlooked high-performing employees  
- Supports data-driven HR policy decisions  
- Enables predictive HR analytics  

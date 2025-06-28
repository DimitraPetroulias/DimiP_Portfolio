# Mapping Employee Satisfaction: Clustering, Prediction and Sentiment Insights

## Overview
This project explores the drivers of employee satisfaction to inform retention strategies and reduce recruitment costs.  
Analyses included:
- **K-means clustering** to identify employee segments.
- **Decision tree modelling** to predict satisfaction.
- **Sentiment analysis** of open-ended feedback.

## Objectives
1. Identify employee groups with similar satisfaction and income levels.
2. Build a model predicting satisfaction based on demographics.
3. Analyse sentiment in employee comments to uncover key themes.

## Data
**File:** `employee_satisfaction_data.csv`  
**Observations:** 142 rows, 9 columns  
Variables include:
- Demographics: Age, Gender, Education, Business Travel, Income, Tenure
- Satisfaction Score
- Open-ended Review

## Tools & Technologies
- **Python** (Jupyter Notebook)
- Key libraries:
  - `pandas`, `numpy` – data cleaning & preparation
  - `matplotlib`, `seaborn` – visualisation
  - `sklearn` – clustering & decision trees
  - `nltk`, `textblob` – sentiment analysis

## Methodology
1. **Data Preprocessing**
   - Convert categorical variables to numeric
   - Standardise continuous variables
   - Handle missing values and outliers
2. **Exploratory Analysis**
   - Descriptive statistics and correlations
   - Visualise distributions and relationships
3. **K-Means Clustering**
   - Determine optimal clusters (Elbow & Silhouette methods)
   - Profile clusters by satisfaction, travel, income, and education
4. **Decision Tree Modelling**
   - Predict satisfaction (satisfied vs dissatisfied)
   - Evaluate and prune the model for interpretability
5. **Sentiment Analysis**
   - Tokenise, lemmatise, and clean text
   - Visualise word frequencies and sentiment distribution
   - Compare TextBlob and NLTK Vader outputs

## Key Findings
- **Clusters:**
  - Frequent travellers reported the lowest satisfaction.
  - Senior employees with high income and tenure had the highest satisfaction.
- **Predictors:**
  - Travel frequency, income, age, and tenure were strongest predictors.
- **Sentiment:**
  - Positive comments focused on flexibility and income.
  - Negative comments emphasised travel burden, low pay, and poor management.

## Recommendations
- Reduce travel requirements for mid-level employees.
- Improve career development and compensation for newer staff.
- Maintain retention strategies for senior employees.
- Continue collecting feedback to monitor satisfaction over time.

## Full Report
For a detailed explanation of this project, you can read the complete report here:  
[Project 2-2 Report (PDF)](https://github.com/DimitraPetroulias/DimiP_UniPortfolio/blob/f87194948a5746da0978ec546392d404b094c4e9/Analysis%20of%20Employee%20Data/Project%202-2%20Report.pdf)

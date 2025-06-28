# Analysing Organisational Climate Drivers of Employee Turnover

## Overall Business Goal
Reduce recruitment costs and minimise the loss of experienced employees by fostering a more positive organisational climate.  
This project identifies dissatisfaction areas, analyses climate factors, and predicts key drivers of organisational climate.

The People and Culture team collected employee satisfaction data using the Organisational Climate Measure (OCM), covering ten dimensions:
- Involvement in decision-making
- Autonomy
- Relationship with direct manager
- Feeling part of a team
- Welfare
- Training
- Work-life balance
- Organisation’s response to change
- Innovation
- Customer orientation

## Objectives
1. Identify the OCM dimension(s) with the lowest scores indicating potential dissatisfaction.
2. Analyse the relationship between overall organisational climate (OC) scores and:
   - Work location, tenure, management responsibilities, intention to quit, and employee sentiment.
   - The ten OCM dimensions.
3. Predict which factors most significantly impact the overall OC score to target improvements and increase retention.

## Data Source
**File:** `employee_survey.csv`

| Variable Name   | Description                                                 | Options                                                   |
|-----------------|-------------------------------------------------------------|-----------------------------------------------------------|
| id              | Unique respondent ID                                        | N/A                                                       |
| agree           | Permission to use data                                      | yes = 1, no = 2                                           |
| workloc         | Main workplace                                              | office = 1, remote = 2                                    |
| workleng        | Length of tenure                                            | 0–5 yrs = 3, 6–10 = 8, 11–15 = 13, 16–20 = 18, >20 = 23   |
| manag_resp      | Management responsibility                                   | yes = 1, no = 2                                           |
| involved        | Involvement in decision-making                              | -5 (very dissatisfied) to +5 (very satisfied)            |
| autonomy        | Trusted to work independently                               | -5 to +5                                                  |
| direct_manag    | Relationship with direct manager                            | -5 to +5                                                  |
| integrated      | Feeling part of a team                                      | -5 to +5                                                  |
| welfare         | Perception of organisational care                           | -5 to +5                                                  |
| training        | Training adequacy                                           | -5 to +5                                                  |
| work_press      | Work-life balance                                           | -5 to +5                                                  |
| reflexive       | Response to external change                                 | -5 to +5                                                  |
| innovative      | Welcomes and implements innovation                          | -5 to +5                                                  |
| customers       | Response to customer needs                                  | -5 to +5                                                  |

## Tools & Technologies
- **Python** (Jupyter Notebook)

**Libraries Used:**
- `pandas`, `numpy`: Data cleaning and transformation
- `matplotlib`, `seaborn`: Data visualisation
- `scipy.stats`, `statsmodels`: Statistical testing (t-tests, ANOVA, chi-square)
- `sklearn`: Regression modelling and metrics
- Additional modules for diagnostic testing and power analysis

## Methodology
**A. Understand Business Goals**

**B. Data Understanding**
- Import and explore dataset
- Rename columns for clarity

**C. Data Preparation**
- Handle missing, duplicate, incorrect values
- Detect and manage outliers

**D. Data Exploration**
- Visualise distributions (boxplots, histograms)
- Assess skewness and kurtosis
- Calculate descriptive statistics
- Rank OCM dimensions by mean score
- Compare overall OC across demographic groups

**E. Analysis and Modelling**
- **Goal 1:** Calculate and rank mean scores of OCM dimensions
- **Goal 2:**
  - Use t-tests and ANOVA to compare OC across:
    - Work location
    - Tenure
    - Management responsibilities
    - Intention to quit
    - Sentiment
  - Perform regression to assess predictors of OC
- **Goal 3:** Develop predictive models identifying key factors influencing OC

## Results
- **Key Issues:** Low scores in team integration and training.
- **Drivers of Climate:** Sense of belonging, autonomy, and manager relationships most strongly influence perceptions.
- **Tenure Matters:** Longer-tenured employees report higher satisfaction; other factors showed no clear impact.

## Recommendations
- **Strengthen Team Integration:**
  - Promote open communication, collaboration, team-building, inclusivity, and onboarding.
- **Enhance Training:**
  - Offer job-specific training, skill development, and resources.
- **Improve Surveys:**
  - Use a 1–5 Likert scale and increase sample size for more reliable insights.

## Full Report
For a detailed explanation of this project, you can read the complete report here:  
[Project 2-1 Report (PDF)](https://github.com/DimitraPetroulias/DimiP_UniPortfolio/blob/aca96a411dd8b0bf29e73b3f2dae7d60d837b887/Analysis%20of%20Employee%20Data/Project%202-1%20Report.pdf)


# Flight Delay Dashboard Development with Tableau

## Overall Business Goal
Provide actionable insights to improve customer experience, service quality, and operational efficiency for a company specialising in last-minute weekend flights across the USA.  
This project develops interactive Tableau dashboards tailored to the needs of customer service and customer success teams, focusing on identifying delay patterns, predicting future disruptions, and supporting data-driven decisions.

## Objectives
1. Develop separate Tableau dashboards for:
   - **Customer Service Team:** To provide accurate, real-time information to passengers about the best travel times, most reliable airlines, and least disrupted routes.
   - **Customer Success Team:** To identify delay trends, understand causes, track airline performance, and inform strategic planning.
2. Integrate and clean historical flight data to ensure robust, reliable visual analysis.
3. Explore predictive models to estimate delay patterns based on flight volumes and times.

## Data Source
**Files:**
- `Flights_from_Atlanta.xls` – Historical flight records departing Atlanta Hartsfield–Jackson International Airport (ATL) in 2015
- `Airlines` – Airline IATA codes and names
- `Airports` – Airport codes and locations
- `USAstates` – US state names and abbreviations

| File                   | Description                                               |
|------------------------|-----------------------------------------------------------|
| Flights_from_Atlanta   | 107,947 rows of flight data covering Friday–Monday travel |
| Airlines               | Airline reference table                                   |
| Airports               | Airport reference table                                   |
| USAstates              | State names and abbreviations                             |

## Tools & Technologies
- **Tableau:** Dashboard design, interactive visualisation, and predictive modelling
- **Python:** Data cleaning, anomaly detection, and validation
- **Excel:** Initial data inspection and transformations

## Methodology

**A. Understand Business Goals**

**B. Data Preparation**
- Validated data integrity:
  - Verified missing values and inconsistencies
  - Confirmed all flights departed ATL
  - Addressed missing latitude and longitude entries
- Created calculated fields in Tableau for:
  - Unified date fields
  - Accurate timestamp columns
  - Delay classification (On-Time, Delayed, Early)

**C. Dashboard Development**
- Developed **two separate dashboards:**
  - **Customer Service Dashboard**:
    - Visualises average delays by month, weekday, and time of day
    - Identifies most and least reliable airlines
    - Highlights least busy destinations
    - Provides weather delay insights
  - **Customer Success Dashboard**:
    - Analyses market share by airline
    - Examines delay causes and trends over time
    - Evaluates airline performance by punctuality
    - Assesses impact of flight volume on delays
- Ensured visual clarity and accessibility (colour-blind palettes, clear typography)

**D. Predictive Modelling**
- Developed regression models to forecast delays based on flight numbers
- Evaluated model fit using:
  - R-squared
  - Mean Squared Error (MSE)
  - p-values
- Established relationships between flight volumes and total delays

**E. Deployment Planning**
- Defined steps for:
  - Design validation and stakeholder engagement
  - Training and support resources
  - Ongoing feedback collection and dashboard iteration

## Results
- **Key Findings:**
  - Late Aircraft and Airline delays were the most common causes.
  - Strong positive correlation between flight numbers and total delays.
  - Peak delays occurred during afternoon and weekend flights.
  - Airline performance varied significantly, with some carriers demonstrating high punctuality.
- **Predictive Models:**
  - Reliable linear models predicting total delays from flight counts (R² > 0.86 for most delay types).
  - Weaker predictive power for security and weather-related delays.

## Recommendations
- **Operational Improvements:**
  - Collaborate with airlines to reduce late aircraft turnaround times.
  - Target infrastructure improvements at peak times and locations.
- **Customer Communication:**
  - Provide clear guidance on optimal travel times and carriers.
  - Offer proactive delay notifications based on predictive models.
- **Ethical Considerations:**
  - Maintain transparency about data usage.
  - Implement robust data governance and access controls.
  - Ensure compliance with Web Content Accessibility Guidelines (WCAG).

## Dashboard Preview
![Tableau Customer Service Team Dashboard](https://github.com/user-attachments/assets/798218c7-e72e-4591-bcb2-9a6ecedbbf86)
![Tableau Customer Success Team Dashboard](https://github.com/user-attachments/assets/5ac56582-ab4a-4e06-818b-3407a623cea5)


## Full Report
For a detailed explanation of the methodology and results, you can read the complete report here:  
[Project 4 – Report (PDF)](https://github.com/DimitraPetroulias/DimiP_UniPortfolio/blob/60fc4a131858900a0b477109b2f7114d2907724b/Flight%20Delay%20Dashboards/Project%204%20Report.pdf)


---


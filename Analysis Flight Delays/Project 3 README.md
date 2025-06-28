# Analysis and Insights of LAX Flight Delays 2015

## Overall Business Goal
Advise a company specialising in last-minute weekend flights across the USA on how to improve customer experience, enhance service quality, reduce operational costs, and minimise landing and departure bottlenecks.  
This project analyses historical flight delay data to uncover delay patterns by airline, airport, state, time of day, day of the week, and month.

## Objectives
1. Identify the main causes of arrival delays among domestic flights departing Los Angeles International Airport (LAX).
2. Assess how delays vary by:
   - Airline
   - Destination airport and state
   - Number of flights operated
   - Time of day
   - Day of the week
   - Month of the year
3. Provide actionable recommendations to reduce delays and improve passenger satisfaction.

## Data Source
**Files:**
- `flightdata.xls` — Historical flight records, including delay causes
- `airlines.csv` — Airline IATA codes and names
- `airports.csv` — Airport codes and locations
- `USAstates.csv` — State abbreviations and full names

| File          | Description                                              |
|---------------|----------------------------------------------------------|
| flightdata.xls| 24,032 rows of flight records from 2015 departing LAX    |
| airlines.csv  | Airline code reference table                             |
| airports.csv  | Airport code reference table                             |
| USAstates.csv | US state names and abbreviations                         |

## Tools & Technologies
- **Excel**:
  - Data cleaning, transformation, and analysis
  - Pivot tables and formulas to correct and aggregate data
  - Charts to visualise trends
- **Python** (for validation of anomalies)
- **SQLite** (DB Browser) for dataset merging

## Methodology

**A. Understand Business Goals**

**B. Data Understanding**
- Reviewed all four datasets and their relationships
- Identified variable definitions, types, and expected ranges

**C. Data Preparation**
- Cleaned anomalies and missing values:
  - Corrected invalid dates and day-of-week entries
  - Resolved inconsistent airline codes using external flight data sources
  - Verified calculated delay times using arrival and departure timestamps
- Removed irrelevant rows (e.g., flights not departing from LAX)
- Merged datasets in SQLite using left joins to preserve all flight records

**D. Data Exploration**
- Analysed distributions of delay variables (arrival, departure, and causes)
- Used histograms, boxplots, and descriptive statistics to detect outliers
- Visualised delay patterns by airline, airport, and state

**E. Analysis and Modelling**
- **Goal 1:**
  - Compared mean and median arrival delay causes
  - Ranked airlines by delay contribution
- **Goal 2:**
  - Assessed relationships between:
    - Number of flights and total/average delays
    - Time of day and delay frequency
    - Day of the week/month and cumulative delays
  - Calculated Pearson correlation coefficients
- **Goal 3:**
  - Synthesised findings into recommendations for operational improvements

## Results
- **Top Delay Causes:** Late-aircraft and airline delays were the largest contributors to arrival delays.
- ![image](https://github.com/user-attachments/assets/c668709e-4c02-4b7a-a179-7eab946f0252)

- **Airline Performance:** American Eagle and Hawaiian Airlines had the highest average delays despite operating fewer flights; Southwest and SkyWest had the lowest average delays.
- ![image](https://github.com/user-attachments/assets/89ccea0e-5ebc-4e73-ae7b-e4018ab5c986)
- the more flights an airline had the greater the arrival delay
- ![image](https://github.com/user-attachments/assets/3d99fe02-7cbc-4046-91c7-0994f54c636c)
- the busier the airport the more delays

- **Temporal Patterns:**
  - Peak delays occurred between 12 pm–6 pm.
  - ![image](https://github.com/user-attachments/assets/d95bd8c6-cf8b-40eb-96fc-bb8770d410b4)

  - Delays were most common on Thursdays, Fridays, and Sundays.
  - ![image](https://github.com/user-attachments/assets/39f790fd-7525-4e6c-ad84-ad8b0ed55674)

- **Geographic Patterns:** New York and Hawaii reported the highest average delays per flight.
- ![image](https://github.com/user-attachments/assets/bdca4ac0-e5b0-475f-9ef2-cd3cd9299ba3)

## Recommendations
- **Operational Improvements:**
  - Focus on reducing late-aircraft turnaround times and airline-controlled delays (e.g., maintenance and crew scheduling).
- **Infrastructure and Resource Allocation:**
  - Prioritise improvements in states with the highest delays, such as New York and Hawaii.
  - Allocate resources to manage peak times of day and days of the week.
- **Customer Advice:**
  - Encourage passengers to fly earlier in the day and avoid peak travel periods.
  - Prefer airlines with lower historical delays, like SkyWest and Southwest.

## Full Report
For a detailed explanation of this project, you can read the complete report here:  
[Project 3 – Flight Delay Analysis Report (PDF)](https://github.com/DimitraPetroulias/DimiP_UniPortfolio/blob/15e35aa08537cd2c17e53bbec73d1fcc8c5ba90d/Analysis%20Flight%20Delays/Project%203%20Report.pdf)


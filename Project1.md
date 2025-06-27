# Analysis of Streaming Movie Data

## Overall Business Goal
Canopy (a fictional business) wants to offer the best-rated French movies and create movies that are not offered by other streaming services.

### Objectives
- Determine the top 20 best-rated movies offered by genre and age group.

## Data Source
![image](https://github.com/user-attachments/assets/5bc295b4-9184-476b-9eef-768e6ce82ba4)


## Tools & Technologies
- Python (Pandas, NumPy, matplotlib, missingno)
- Jupyter Notebook

## Methodology

The standard methodology utilised:

**A. Understanding the business goals**

**B. Exploring the data to gain an understanding**
- Importing the data and exploring its properties
- Renamed columns

**C. Assessing the quality of the data and rectifying any issues**
- Missing values
- Unique values
- Duplicate values

**D. Filtering and merging the datasets**
- Kept only columns of interest to address business goals
- Merged the two tables using a left outer join

**E. Performing analyses to address the business goals**
- Group by function
- Distribution of genres in each age group and where streamed
- Distribution of number of movies in each age group

## Results
- Provided the top 20 French movies for each genre for Canopy to stream on their service
- Recommended what genres of French movies Canopy should make

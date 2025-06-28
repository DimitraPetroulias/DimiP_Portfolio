# Analysis of Streaming Movie Data Part 2

## Overall Business Goal
Canopy (a fictional business) wants to offer the best-rated French movies and create movies that are not offered by other streaming services.

### Objectives
Their objectives are to:
1. Offer curated selections of best rated French-language movies from the existing content,
2. Provide French-language movies to various age groups,
3. Identify the least tapped genres to provide the filmmakers with data to make original content for Canopy.

These goals were addressed in Project 1. However, we are now required to create a visualisation dashboard to provide insights into the following business questions:

1. Does France make longer movies on average based on runtime?
2. Does France make better movies on average based on ratings?
3. Are there any French-language movies that claim to be of more than one genre?

It was also suggested that Canopy investigate the following:

4. Where is France placed compared to other countries with regard to the number of movies they make?
5. Is there a relationship between age groups and genres for French-language movies?
6. Is there a relationship between Runtime and IMDb rating for French-language movies?

These additional questions will provide further insights into Canopy’s business goals and assist filmmakers in creating original content.
## Data Source
One csv movie file was provided
![image](https://github.com/user-attachments/assets/19ef325e-0704-41ee-8606-794de4ce6d91)


## Tools & Technologies
- Python (Pandas, NumPy, matplotlib, missingno, matplotlib.pyplot, seaborn, bokeh.transform, bokeh.plotting)
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
- Outliers (review distributions)

**D. Filtering and merging the datasets**
- was not required

**E. Performing analyses to address the business goals**
1. **Does France make longer movies on average based on runtime?**
   - Two methods were used to answer this question:
     - **Method 1:** Used the `Country` column, assuming the first country listed is where the movie was made.
     - **Method 2:** Used the `Language` column and filtered for French-language and non-French-language movies.

2. **Does France make better movies on average based on ratings?**
   - Two methods were used to answer this question:
     - **Method 1:** Used the `Country` column, assuming the first country listed is where the movie was made.
     - **Method 2:** Used the `Language` column and filtered for French-language and non-French-language movies.

3. **Are there any French-language movies that claim to be of more than one genre?**
   - Two methods were used to answer this question:
     - **Method 1:** Applied the `split()` method to separate the genres and count the number of genres per movie.
     - **Method 2:** Used the `explode()` method to split the genres into separate rows, then applied `groupby()` to count the number of genres per movie.

4. **Where is France placed compared to other countries regarding the number of movies produced?**
   - Created a histogram to illustrate this comparison.

5. **Is there a relationship between age groups and genres for French-language movies?**
   - Created a histogram to visualise the distribution.

6. **Is there a relationship between runtime and IMDb rating for French-language movies?**
   - Used a scatterplot to explore the correlation.


## Results
The analysis indicates that French-language movies generally have higher IMDb ratings and longer runtimes compared to non-French-language movies, supporting Canopy’s goal of offering curated, highly rated content. Additionally, the diverse range of genres across different age groups allows Canopy to cater to various demographics effectively.

Insights into less tapped genres and the relationship between runtime and IMDb ratings can help filmmakers create original content tailored for Canopy’s audience. Filmmakers are encouraged to focus on genres such as **Biography**, **History**, **Fantasy**, **War**, **Animation**, **Horror**, **Sci-Fi**, **Musical**, **Sport**, **Western**, and **Shorts**, particularly targeting the **16+ age group**.

The decline in French movie production suggests that Canopy should consider producing more French films to maintain a consistent content flow. Furthermore, Canopy can leverage the scarcity of new French films to position itself as a unique platform that not only curates the best existing content but also supports the creation of new, high-quality French-language movies.
 
## Full Report
For a detailed explanation of this project, you can read the complete report here:  
[Project 1-2 Report (PDF)](https://github.com/DimitraPetroulias/DimiP_UniPortfolio/blob/0fa62e7c87992bf44f0f8b913efaa7a51c16bdfb/Analysis%20of%20Streaming%20Movie%20Data/Project%201-2%20Report.pdf)

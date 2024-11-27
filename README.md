
# **Movie Analysis Project**

## **Table of Contents**
1. [Project Overview](#project-overview)  
2. [Key Insights and Visualizations](#key-insights-and-visualizations)  
   - [Profit Margins by Studio](#profit-margins-by-studio)  
   - [Budget vs. Profit Margin](#budget-vs-profit-margin)  
   - [Average Revenue by Genre](#average-revenue-by-genre)  
   - [Revenue by Release Month](#revenue-by-release-month)  
   - [Revenue by Original Language](#revenue-by-original-language)  
   - [Audience Ratings vs. Revenue](#audience-ratings-vs-revenue)  
3. [Interactive Features](#interactive-features)  
4. [Accessing the Dashboard](#accessing-the-dashboard)  
5. [Future Enhancements](#future-enhancements)  
6. [Acknowledgments](#acknowledgments)  

---


## **Project Overview**
In my **Movie Analysis** project, I aimed to uncover pivotal insights into the movie industry by addressing key questions, including:

- Which genres consistently generate the highest revenue?
- How do budgets correlate with worldwide gross?
- What are the most profitable release windows for movies?
- How do audience ratings influence box office success?
- Which studios have the highest profit margins?
- Does the original language of a movie influence its global performance?

My objective was to provide stakeholders with actionable, data-driven insights to guide strategic decisions in movie production and distribution.

---

## **Data Understanding**
To answer these questions, I analyzed multiple datasets, merging and cleaning them to create a unified dataset for analysis. The primary datasets I used were:

### **Datasets**
1. **Box Office Mojo**: Data on box office performance by studio.
2. **The Numbers**: Focused on production budgets and revenues.
3. **Rotten Tomatoes Reviews**: Audience and critic review scores.
4. **Rotten Tomatoes Movie Info**: Metadata, including genres, runtimes, and release dates.
5. **TMDB**: Popularity metrics, genre details, and vote counts.
6. **im.db.zip**: A zipped SQLite database containing `movie_basics` and `movie_ratings` tables for detailed insights into movie ratings and metadata.

### **Actions Taken**
- Cleaned and standardized datasets to address missing values and formatting inconsistencies.
- Merged relevant datasets to form a consolidated, clean dataset for analysis.

### **Key Features in the Data**
- **Revenue Metrics**: Domestic, foreign, and worldwide gross.
- **Production Metrics**: Budget, profit, and profit margins.
- **Movie Details**: Genres, runtimes, release dates, and languages.
- **Audience Insights**: Average ratings and vote counts.

---

## **Questions Answered**
1. **What genres should producers invest in?**
   - Action and adventure movies consistently dominate global revenue.
![alt text](c5b801a3-7044-4f40-9e94-cb82ec99f003.png)
---
2. **Does budget guarantee success?**
   - Higher budgets correlate with revenue, but profitability depends on strategic spending.
![alt text](65759c0a-06f6-46a1-9fee-f5ae4b467fb7.png)
---
3. **Which studios have the highest profit margins?**
   - Top-performing studios like Disney and Universal deliver high profit margins but show significant variability.
![alt text](a38be226-eb14-497c-9008-920174b76873.png)
---
4. **When should movies be released?**
   - Summer and holiday seasons maximize box office revenue.
![alt text](b2bf37e2-1d14-43ae-9fca-50083b97cf30.png)
---
5. **How do audience ratings affect success?**
   - Both higher ratings and vote counts correlate strongly with better box office performance.
![alt text](690f6454-e7ee-4021-9261-b7ec78131d8c.png)![alt text](5b3ebc33-fafd-4070-aa09-ae54e78f49a4.png)
---
6. **How does a movie's original language influence revenue?**
   - English-language movies lead in global revenue, though select non-English films show increasing traction in niche markets.
![alt text](f8af2906-20ca-465f-89ca-1ee1967cb97f.png)
---

## **Graphs and Visualizations**
### Key Visualizations Created:
- **Profit Margins by Studio**: Displays the variability in studio profitability.
- **Budget vs. Profit Margin**: Explores the relationship between budgets and profitability.
- **Average Revenue by Genre**: Highlights top-performing genres globally.
- **Revenue by Release Month**: Shows seasonal trends in box office performance.
- **Revenue by Original Language**: Examines the impact of a movie’s language on global appeal.
- **Audience Ratings vs. Revenue**: Investigates how ratings and votes affect box office performance.

---

## **Tools and Technologies Used**
- **Python**: For data cleaning, analysis, and visualizations.
- **Tableau**: For creating interactive dashboards.
- **Libraries**: Pandas, Seaborn, Matplotlib, and others for statistical and graphical analysis.

---

## **Interactive Dashboards**
Using Tableau, I created dashboards that allow stakeholders to:
- Explore genre-specific revenue trends.
- Identify optimal release windows.
- Compare studio profitability.
- Understand the impact of audience ratings on revenue.

📂 **Access the Tableau Workbook**: *(Insert link here)*

---

## **Files in Repository**
| **File Name**             | **Description**                                      |
|---------------------------|----------------------------------------------------|
| `cleaned_merged_movies.csv` | Preprocessed dataset used throughout the analysis. |
| `Final_Movie_Analysis.ipynb` | Jupyter Notebook with code, analysis, and visualizations. |
| `requirements.txt`        | File listing all Python dependencies.             |
| `Tableau_Workbook.twb`    | Tableau workbook containing all dashboards.        |

---

## **Future Enhancements**
1. **Advanced Predictive Models**:
   - Incorporate techniques like Random Forests or Gradient Boosting for revenue prediction.
2. **Regional Insights**:
   - Include regional box office data for a more comprehensive analysis.
3. **Streaming Platform Trends**:
   - Investigate how streaming services impact box office performance.
4. **Customer Segmentation**:
   - Cluster audiences based on preferences and demographics for targeted marketing.

---

## **Acknowledgments**
This project was inspired by the transformative potential of data in reshaping decision-making in the entertainment industry. Special thanks to:
- The Flatiron School for the foundational dataset.
- The Tableau Public and Python communities for their resources and tools.
```

--

![alt text](movie-3057394_1280-1.jpg)

## **Project Overview**

In my **Movie Analysis** project, I set out to address pivotal questions about the movie industry, such as:  
- Which genres consistently generate the highest revenue?  
- How do budgets correlate with worldwide gross?  
- What are the most profitable release windows for movies?  
- How do audience ratings influence box office success?  
- Can I use movie attributes to predict revenue?  

My goal was to empower stakeholders in the movie industry to make data-driven decisions by uncovering actionable insights.  

---

# **Data Understanding**

To uncover trends and patterns in the movie industry, I analyzed multiple datasets from various sources. Below, I outline the key datasets I worked with, their features, and the challenges I resolved during my analysis:

---

## 1. **Box Office Mojo Data**

**Overview**: This dataset provided information on box office revenue and studio details.  

- **Shape**: 3,387 rows and 5 columns.

### Columns:
- **title**: Movie title (non-null).  
- **studio**: Studio responsible for the movie (5 missing values).  
- **domestic_gross**: Domestic gross earnings (28 missing values).  
- **foreign_gross**: Foreign gross earnings (1,350 missing values, stored as strings).  
- **year**: Release year (non-null).  

### Actions I Took:
- Converted `foreign_gross` from strings to numeric format to enable accurate calculations.  
- Resolved missing values in the `studio` and revenue columns using context-driven techniques.  

---

## 2. **The Numbers Data**

**Overview**: This dataset focused on production budgets, domestic, and worldwide gross revenues.  

- **Shape**: 5,782 rows and 6 columns.

### Columns:
- **id**: Unique identifier for each movie (non-null).  
- **release_date**: Movie release date (non-null).  
- **movie**: Movie title (non-null).  
- **production_budget**: Production budget (stored as strings with commas, required conversion).  
- **domestic_gross** and **worldwide_gross**: Revenue columns stored as strings with commas.  

### Actions I Took:
- Cleaned and converted all budget and revenue columns into numeric format for easier analysis.  
- Preprocessed string data to ensure consistency, even though there were no missing values.  

---

## 3. **Rotten Tomatoes Reviews Data**

**Overview**: This dataset included reviews, ratings, and publisher information for movies.  

- **Shape**: 54,432 rows and 8 columns.

### Columns:
- **id**: Unique identifier for movies (non-null).  
- **review**: Textual review (5,563 missing values).  
- **rating**: Rating given by critics (13,517 missing values).  
- **fresh**: Binary indicator of whether a review is "fresh" or "rotten" (non-null).  
- **critic**: Name of the critic (2,722 missing values).  
- **top_critic**: Flag indicating whether the reviewer is a top critic (non-null).  
- **publisher**: Publisher of the review (309 missing values).  
- **date**: Date of the review (non-null).  

### Actions I Took:
- Analyzed missing data in the `review`, `rating`, and `critic` columns to decide their impact on analysis.  
- Focused on columns that directly contributed to answering project goals, deprioritizing less relevant ones.  

---

## 4. **Rotten Tomatoes Movie Info Data**

**Overview**: This dataset provided metadata such as genres, directors, runtime, and box office data.  

- **Shape**: 1,560 rows and 12 columns.

### Columns:
- **id**: Unique identifier (non-null).  
- **synopsis**: Movie synopsis (62 missing values).  
- **rating**: MPAA rating (3 missing values).  
- **genre**: Movie genre (8 missing values).  
- **director**: Director name (199 missing values).  
- **writer**: Writer name (449 missing values).  
- **theater_date**: Theater release date (359 missing values).  
- **dvd_date**: DVD release date (359 missing values).  
- **currency** and **box_office**: Sparse columns with very limited non-null values.  
- **runtime**: Runtime of the movie (30 missing values).  
- **studio**: Studio responsible (very sparse).  

### Actions I Took:
- Noted and accounted for the sparse data in `studio`, `currency`, and `box_office`, which limited their use.  
- Focused on `rating`, `genre`, `director`, and `runtime` for genre-based and attribute-specific analysis.  

---

## 5. **TMDB Data**

**Overview**: This dataset covered popularity metrics, genre information, vote averages, and counts.  

- **Shape**: 26,517 rows and 10 columns.

### Columns:
- **id**: Unique identifier (non-null).  
- **genre_ids**: List of genre IDs for each movie (non-null).  
- **original_language**: Language of the movie (non-null).  
- **original_title** and **title**: Original and common titles (non-null).  
- **popularity**: Popularity score (non-null).  
- **release_date**: Movie release date (non-null).  
- **vote_average** and **vote_count**: Average audience rating and number of votes (non-null).  

### Actions I Took:
- Decoded `genre_ids` into human-readable genres to improve interpretability.  

---

## **Dataframes for Analysis**

After reviewing the datasets, I prioritized the following for analysis:

1. **Box Office Mojo Data**: Analyzed box office trends, domestic vs. international performance, and studio impact.  
2. **The Numbers Data**: Investigated the relationship between budgets and revenues.  
3. **Rotten Tomatoes Movie Info Data**: Explored genres, directors, and runtime as factors influencing box office success.  
4. **TheMovieDB Data**: Analyzed audience popularity, vote averages, and their relationship to revenue.

---

## **Key Features and Insights**

### Analysis Highlights:
1. **Genre Trends**: Action and adventure movies consistently lead in revenue generation.  
2. **Budget vs. Revenue**: Higher budgets often correlate with greater revenues, but profitability depends on strategic budgeting.  
3. **Seasonal Insights**: Summer and holiday releases perform best, while off-season movies tend to underperform.  
4. **Audience Ratings**: Higher audience ratings and vote counts strongly correlate with box office success.  
5. **Predictive Model**: I developed a regression model to predict worldwide gross based on budget, ratings, and other features.

---

## **Tools and Technologies Used**

- **Python**: Data cleaning, exploratory analysis, and model development.  
- **Tableau**: Interactive visualizations for better insights.  
- **Key Libraries**: Pandas, Matplotlib, Seaborn, Scikit-Learn.  

---

## **Installation and Setup**

### Requirements:
- Python 3.8 or higher  
- Libraries: Pandas, Matplotlib, Seaborn, Scikit-Learn, Jupyter Notebook  

### Steps:
1. Clone the repository to your local machine:  
   ```bash
   git clone https://github.com/your-repo/movie-data-analysis.git
   ```  
2. Navigate to the project directory:  
   ```bash
   cd movie-trends-analysis
   ```  
3. Install all required libraries using the provided `requirements.txt` file:  
   ```bash
   pip install -r requirements.txt
   ```  
4. Launch the Jupyter Notebook to explore the analysis and model:  
   ```bash
   jupyter notebook Movie_data_Analysis.ipynb
   ```  

   ## **Data Analysis Highlights**

### Questions Addressed:
1. **What genres should producers invest in?**  
   - Action and adventure consistently dominate the box office.  
2. **Does budget guarantee success?**  
   - While higher budgets correlate with revenue, strategic allocation is essential for profitability.  
3. **When should movies be released?**  
   - Summer and holiday seasons deliver the highest returns.  
4. **How important are audience ratings?**  
   - Higher ratings and vote counts strongly correlate with better box office performance.  

### Graphs:
- **Bar Chart**: Revenue performance across genres.  
- **Scatter Plot**: Relationship between budget and worldwide gross.  
- **Bar Chart**: Seasonal trends in revenue generation.  

---


### **Interactive Dashboards**
  
With the Tableau dashboards, users can:  
- **Dive into Genre-Specific Performance**: Identify the most profitable genres and tailor production strategies.  
- **Explore Seasonal Trends to Identify Optimal Release Windows**: Discover the best times to release movies for maximum box office impact.  
- **Compare Actual Revenue Against Predicted Values**: Analyze performance metrics and identify key outliers or trends for refining budgets.

📂 **Access the Tableau Workbook**:  
   - [Click here to access the workbook](#) *(Insert actual link or instructions for download)*  

---

### **Files in Repository**

| File Name                    | Description                                                   |
|------------------------------|---------------------------------------------------------------|
| `cleaned_merged_movies.csv`  | The preprocessed dataset used in all stages of the analysis.  |
| `Final_Movie_Analysis.ipynb` | Jupyter Notebook with code, analysis, and visualizations.     |
| `requirements.txt`           | File listing all Python dependencies required for execution.  |
| `Tableau_Workbook.twb`       | Tableau workbook containing all dashboards and insights.      |

---

### **Future Enhancements**

1. **Advanced Predictive Models**:
   - Incorporate algorithms like Random Forests, Gradient Boosting, or Neural Networks to forecast revenue trends more accurately.

2. **Incorporate External Factors**:
   - Analyze how market competition, social media trends, or the influence of streaming platforms impact revenue.

3. **Regional Insights**:
   - Expand the dataset to include revenue and audience trends from regional and global markets for a more comprehensive analysis.

4. **Customer Segmentation**:
   - Cluster moviegoers by preferences, demographics, or spending habits to tailor marketing campaigns.

---

### **Acknowledgments**

This project was inspired by the transformative potential of data in reshaping decision-making within the entertainment industry.  
- The dataset was adapted from the **Flatiron School GitHub repository** and served as the foundation for all analyses.  
- Special thanks to the **Tableau Public and Python communities** for their tools and guidance in creating visualizations and models.

---

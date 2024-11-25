![alt text](movie-3057394_1280-1.jpg)

## **Project Overview**

In my **Movie Analysis** project, I set out to address pivotal questions about the movie industry, such as:  
- Which genres consistently generate the highest revenue?  
- How do budgets correlate with worldwide gross?  
- What are the most profitable release windows for movies?  
- How do audience ratings influence box office success?  
- Which studios have the highest profit margins?  
- Does the original language of a movie influence its global performance?  
- Can I use movie attributes to predict revenue?  

My goal was to empower stakeholders in the movie industry to make data-driven decisions by uncovering actionable insights.

---

## **Data Understanding**

To uncover trends and patterns in the movie industry, I analyzed multiple datasets from various sources. Below, I outline the key datasets I worked with, their features, and the challenges I resolved during my analysis:

---

### **Datasets**
1. **Box Office Mojo Data**: Box office performance by studio.  
2. **The Numbers Data**: Focused on budgets and revenues.  
3. **Rotten Tomatoes Reviews Data**: Audience and critic review scores.  
4. **Rotten Tomatoes Movie Info Data**: Metadata, including genres, runtime, and release dates.  
5. **TMDB Data**: Popularity metrics, genre insights, and vote data.

**Actions Taken**:  
- Standardized and cleaned all datasets to handle missing values and inconsistent data formatting.  
- Merged relevant datasets to create a consolidated dataset for analysis.  

---

## **Dataframes for Analysis**

The following datasets were prioritized to answer specific questions:  
- **Box Office Mojo**: Studio performance and revenue trends.  
- **The Numbers**: Budget and revenue correlations.  
- **Rotten Tomatoes Movie Info**: Genre, director, and runtime analysis.  
- **TMDB**: Popularity, ratings, and language performance trends.

---

## **Key Features and Insights**

### Questions Addressed:
1. **What genres should producers invest in?**  
   - Action and adventure movies consistently dominate the box office.  
2. **Does budget guarantee success?**  
   - While higher budgets correlate with revenue, profitability relies on strategic allocation.  
3. **Which studios have the highest profit margins?**  
   - Top studios like Disney and Universal outperform others consistently, with significant variability.  
4. **When should movies be released?**  
   - Summer and holiday seasons are optimal for maximizing revenue.  
5. **How do audience ratings affect success?**  
   - Higher ratings and vote counts strongly correlate with better box office performance.  
6. **How does a movie's original language influence revenue?**  
   - Movies in English generate the highest worldwide gross, but non-English films are gaining traction.  
7. **How can we predict movie revenue?**  
   - Using production budgets, genres, release months, and audience ratings, predictive models provide actionable forecasts.

---

### **Graphs and Visualizations**

Here are some of the **key visualizations** created in the project:

1. **Profit Margins by Studio** (Box Plot):  
   - Displays variability in profitability among studios.
   - **Question Answered**: "Which studios deliver the highest profit margins?"  

2. **Budget vs. Profit Margin** (Scatter Plot):  
   - Examines the correlation between production budgets and profitability.
   - **Question Answered**: "Do bigger budgets guarantee profitability?"  

3. **Average Revenue by Genre** (Bar Chart):  
   - Highlights top-performing genres globally.
   - **Question Answered**: "Which genres generate the highest revenue?"  

4. **Revenue by Release Month** (Line Chart):  
   - Seasonal trends in box office performance.
   - **Question Answered**: "When is the best time to release movies?"  

5. **Revenue by Original Language** (Bar Chart):  
   - Explores the impact of movie language on global performance.
   - **Question Answered**: "Does the original language of a movie influence its global appeal?"  

6. **Audience Ratings vs. Revenue** (Scatter Plot):  
   - Investigates the relationship between audience approval and box office performance.
   - **Question Answered**: "How important are ratings and votes for box office success?"

---

### **Tools and Technologies Used**

- **Python**: For data cleaning, analysis, and modeling.  
- **Tableau**: For creating interactive and impactful visualizations.  
- **Libraries**: Pandas, Seaborn, Matplotlib, Scikit-learn for machine learning models.

---

## **Interactive Dashboards**

With the Tableau dashboards, users can:  
- Explore **Genre-Specific Trends** to identify high-performing movie categories.  
- Discover **Seasonal Patterns** for optimizing release schedules.  
- Compare **Studio Profitability** to guide collaboration and investments.  
- Evaluate the **Impact of Ratings** on box office success.

📂 **Access the Tableau Workbook**:  
   - [Click here to access the workbook](#) *(Insert link here)*  

---

### **Future Enhancements**

1. **Advanced Predictive Models**:  
   - Incorporate algorithms like Random Forest and Gradient Boosting for better accuracy.  

2. **Regional Insights**:  
   - Expand the dataset to include country-specific box office data.  

3. **Streaming Trends**:  
   - Explore how the rise of streaming platforms affects movie profitability.  

---

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


# Detailed Report – Board Games Data Analysis

## Project Title:
Analysis and Cleaning of Board Games Dataset

## Project Description:
This project aims to analyze a dataset containing information about various board games. The core objective is to clean the data, handle missing values and outliers, explore the distribution of key variables, and identify meaningful insights related to game ratings and popularity. The entire workflow is performed using Python and essential data analysis libraries.

---

## Tools and Technologies:
- **Python 3.x**
- **Jupyter Notebook**
- **Libraries Used**:
  - pandas (data manipulation)
  - matplotlib (data visualization)
  - seaborn (statistical graphics)

---

## Dataset Overview:
The dataset consists of metadata about board games, including:
- Game names
- Year published
- Minimum and maximum number of players
- Playtime duration
- Age requirements
- Number of users who rated the game
- Average rating

---

## Data Cleaning Process:
- **Dropped Irrelevant Columns**: Columns that were not useful in analysis (e.g., image URLs or game IDs) were removed.
- **Handling Missing Values**: Rows with null values in critical columns like `average_rating` or `users_rated` were dropped.
- **Type Conversion**: Data types were corrected where necessary, such as converting the `year_published` to integer.
- **Filtering Zero-Rated Games**: Games that received zero ratings were filtered out to improve result accuracy.

---

## Handling Outliers:
Outliers were identified using statistical summaries and visualization tools:
- **Box Plots and Histograms** were used to detect skewed data points.
- Games with unusually high `users_rated` or `average_rating` were visually inspected.
- Some outliers were retained as they reflected popular or top-rated games.
- Others were excluded when they distorted the overall patterns.

---

## Exploratory Data Analysis (EDA):
### 1. Distribution of Average Ratings
- Most games have an average rating between 5 and 8.
- Very few games received either extremely low or extremely high ratings.

### 2. Relationship Between Users Rated and Rating
- Strong positive correlation observed.
- Games with more user reviews tend to have higher average ratings, possibly due to broader exposure and popularity.

### 3. Ratings vs. Year Published
- A slight trend indicating that recently published games tend to receive higher ratings.
- This may be due to modern game mechanics or broader community reach.

### 4. Correlation Heatmap
- Highlighted strong correlation between `users_rated` and `average_rating`.

---

## Key Insights:
- The number of user reviews is a reliable predictor of a game’s rating.
- Modern board games are generally more popular and better rated.
- Data cleaning significantly enhanced the reliability of the analysis.
- Not all outliers are noise; some represent exceptionally popular games.

---

## Challenges Faced:
- Missing data in important fields.
- Imbalanced distribution due to zero-rated or unrated games.
- Visualizing large variance in user ratings across different game types.

---

## Recommendations:
- Further investigation into genre-specific game ratings.
- Use natural language processing to analyze user reviews (if available).
- Build a predictive model to estimate ratings based on other features.
- Develop an interactive dashboard for better visualization using Power BI or Tableau.

---

## Conclusion:
This project provided a comprehensive view of board game data and demonstrated how to transform raw data into meaningful insights through proper cleaning and analysis. It highlighted the importance of data preparation and exploration in driving actionable conclusions.

---

**Prepared by: Asmaa – Junior Data Analyst**  
This project is intended as a portfolio piece to showcase capabilities in real-world data analysis using Python and visual analytics.

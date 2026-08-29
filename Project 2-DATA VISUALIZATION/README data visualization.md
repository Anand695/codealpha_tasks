# codealpha-tasks
# 🎬 Netflix Movies & TV Shows — Data Visualization Project

## 📌 Project Overview

This project performs an exploratory data analysis and visualization of Netflix Movies and TV Shows using two separate datasets.

The two datasets are combined and analyzed to identify patterns in:

- Audience engagement
- Genre popularity
- Content-producing countries
- Ratings
- Popularity
- Budget and revenue
- Relationships between important variables

The project focuses on creating clear and meaningful visualizations that make differences and patterns in Netflix content easier to understand.

---

## 🎯 Objectives

The main objectives of this project are:

1. Analyze Netflix Movies and TV Shows using data visualization.
2. Compare audience engagement between Movies and TV Shows.
3. Identify the most common and most audience-engaged genres.
4. Analyze the countries producing the most Netflix content.
5. Study rating and popularity distributions.
6. Examine the relationship between ratings and popularity.
7. Analyze the relationship between production budget and revenue.
8. Identify the most popular titles.
9. Generate data-driven insights and recommendations.

---

## 📂 Dataset

The project uses two CSV files:

- `netflix_movies_detailed_up_to_2025.csv`
- `netflix_tv_shows_detailed_up_to_2025.csv`

Both datasets are loaded separately and then combined into a single DataFrame for analysis.

A `content_type` column is created to distinguish between:

- Movie
- TV Show

---

## 🛠️ Technologies Used

- **Python**
- **Google Colab**
- **Pandas** — Data manipulation and analysis
- **NumPy** — Numerical operations
- **Matplotlib** — Data visualization
- **Seaborn** — Statistical visualization

---

## 🧹 Data Cleaning & Preprocessing

The following preprocessing steps were performed:

- Combined Movies and TV Shows datasets
- Removed duplicate records
- Converted numerical columns to appropriate numeric types
- Handled missing categorical values
- Converted release dates into datetime format
- Filled missing numerical values where appropriate
- Created a `decade` feature from release year
- Created a `content_age` feature
- Split and expanded genre information
- Split and expanded country information

---

## 📊 Visualizations & Analysis

### 1. Audience-Engaged Content Type

A **donut/ring chart** is used to compare the total audience engagement between Movies and TV Shows.

Since actual Netflix watch-time data is not provided, `vote_count` is used as an **audience-engagement proxy**.

This helps identify which type of content receives greater audience interaction.

---

### 2. Top 10 Genres by Number of Titles

A bar chart identifies the most frequently represented genres in the dataset.

This helps understand Netflix's content composition and which genres have the largest presence.

---

### 3. Movies vs TV Shows Across Major Genres

The major genres are compared based on their Movie and TV Show representation.

This highlights which genres are more strongly associated with Movies or TV Shows.

---

### 4. Most Audience-Engaged Genres

Genres are ranked using total viewer votes.

This identifies genres that receive the highest level of audience interaction based on the available data.

---

### 5. Average Popularity by Genre

The average popularity of genres is calculated and compared.

Only genres with a sufficient number of titles are considered to avoid misleading results from very small samples.

---

### 6. Rating Distribution

A box plot compares the rating distributions of Movies and TV Shows.

It helps identify:

- Median ratings
- Spread of ratings
- Possible outliers
- Differences between Movies and TV Shows

---

### 7. Popularity Distribution

A box plot is used to compare the popularity distributions of Movies and TV Shows.

Extreme popularity values are limited using a percentile-based approach to make the visualization easier to interpret.

---

### 8. Rating vs Popularity

A scatter plot examines the relationship between:

- Average Rating
- Popularity

Movies and TV Shows are differentiated to identify whether highly rated content also tends to have higher popularity.

---

### 9. Top 10 Content-Producing Countries

A bar chart identifies the countries contributing the largest number of titles.

This provides insight into the geographical distribution of Netflix content.

---

### 10. Movies vs TV Shows Across Major Countries

Major content-producing countries are compared based on their Movie and TV Show representation.

This helps identify differences in content formats across countries.

---

### 11. Production Budget vs Revenue

A scatter plot analyzes the relationship between production budget and revenue.

This can help identify whether higher production investments are associated with higher revenues among titles where financial data is available.

A logarithmic scale is used because budget and revenue values can vary substantially.

---

### 12. Top 10 Most Popular Titles

The project identifies the 10 titles with the highest popularity values.

This provides a quick view of the most prominent titles according to the dataset's popularity metric.

---

### 13. Correlation Heatmap

A correlation heatmap examines relationships between:

- Release Year
- Popularity
- Vote Count
- Vote Average
- Budget
- Revenue

This helps identify variables that show stronger positive or negative relationships.

---

## 📈 Key Insights

The analysis automatically generates important findings, including:

- Most audience-engaged content type
- Most common genre
- Most audience-engaged genre
- Leading content-producing country
- Differences between Movies and TV Shows
- Relationship between ratings and popularity
- Relationship between budget and revenue

The exact values are generated dynamically when the notebook is executed.

---

## 💡 Data-Driven Recommendations

Based on the analysis, the project provides recommendations such as:

- Focus on genres showing strong audience engagement and popularity.
- Use country-level trends to identify strong regional content markets.
- Consider ratings, popularity and viewer votes together instead of relying on a single metric.
- Analyze budget-revenue relationships before making major production investments.
- Identify highly engaged but underrepresented genres as potential content opportunities.

---

## ⚠️ Important Note About Audience Engagement

The datasets do not contain actual Netflix viewing hours or number of streams.

Therefore, **`vote_count` is used as a proxy for audience engagement**.

This means the audience-engagement analysis represents audience interaction reflected by the available voting data, rather than actual Netflix watch-time.

---

## 🚀 How to Run the Project

### Step 1 — Open Google Colab

Upload/open the project notebook in Google Colab.

### Step 2 — Upload the datasets

Upload both CSV files into the Colab environment:

```text
netflix_movies_detailed_up_to_2025.csv
netflix_tv_shows_detailed_up_to_2025.csv

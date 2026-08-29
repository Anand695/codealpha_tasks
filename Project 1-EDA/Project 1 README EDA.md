# 📊 Student Academic Performance Analysis – Exploratory Data Analysis

## 📌 Project Overview

This project was developed as part of the **Data Analytics Internship at CodeAlpha**.

The project focuses on performing **Exploratory Data Analysis (EDA)** on the **Student Performance Factors** dataset to understand the factors associated with students' examination performance.

The analysis explores academic, behavioral, and lifestyle factors and investigates their relationships with students' **Exam Score**.

---

## 🎯 Objectives

The main objectives of this project are:

- Understand the structure and characteristics of the dataset.
- Identify and handle data quality issues.
- Analyze the distribution of important variables.
- Identify trends, patterns, and anomalies.
- Examine relationships between different student factors and Exam Score.
- Perform correlation analysis.
- Test statistical hypotheses using Pearson correlation and p-values.
- Compare the characteristics of the Top 10% and Bottom 10% performing students.
- Present findings through clear and meaningful visualizations.

---

## ❓ Key Questions

The analysis attempts to answer the following questions:

1. Does studying for more hours relate to higher Exam Scores?
2. Does higher attendance relate to better examination performance?
3. Is previous academic performance associated with current Exam Score?
4. Do tutoring sessions show a relationship with Exam Score?
5. Is sleep duration associated with examination performance?
6. Is physical activity associated with Exam Score?
7. Which factors have the strongest relationship with Exam Score?
8. How different are the Top 10% and Bottom 10% performing students?
9. Are there any unusual or anomalous observations in the dataset?
10. Are the observed relationships statistically significant?

---

## 📂 Dataset

**Dataset:** Student Performance Factors

The dataset contains information related to students' academic habits, lifestyle, and other factors that may be associated with examination performance.

### Important Variables

| Variable | Description |
|---|---|
| `Hours_Studied` | Number of hours studied |
| `Attendance` | Student attendance percentage |
| `Previous_Scores` | Previous academic score |
| `Sleep_Hours` | Number of hours slept |
| `Tutoring_Sessions` | Number of tutoring sessions |
| `Physical_Activity` | Physical activity level |
| `Exam_Score` | Final examination score |

The dataset also contains additional demographic, academic, and behavioral variables.

---

## 🛠️ Tools & Technologies

The project was implemented using:

- **Python**
- **Google Colab**
- **Pandas**
- **NumPy**
- **Matplotlib**
- **Seaborn**
- **SciPy**

---

## 📊 Analysis Performed

### 1. Data Understanding

- Dataset shape
- Column names
- Data types
- Statistical summary
- Dataset information

### 2. Data Cleaning

- Missing value detection
- Duplicate detection
- Handling missing values
- Checking data quality

### 3. Univariate Analysis

Distribution analysis was performed for variables such as:

- Exam Score
- Hours Studied
- Sleep Hours

### 4. Relationship Analysis

The following relationships were investigated:

- Hours Studied vs Exam Score
- Attendance vs Exam Score
- Previous Scores vs Exam Score
- Sleep Hours vs Exam Score
- Tutoring Sessions vs Exam Score
- Physical Activity vs Exam Score

### 5. Correlation Analysis

A correlation matrix and heatmap were created to identify the strength and direction of relationships between numerical variables.

### 6. Outlier & Anomaly Detection

The **Interquartile Range (IQR)** method was used to identify potentially unusual observations.

### 7. Hypothesis Testing

Pearson correlation and p-values were used to statistically evaluate selected relationships.

The significance level used was:

**α = 0.05**

- If `p < 0.05` → Reject the null hypothesis.
- If `p ≥ 0.05` → Fail to reject the null hypothesis.

### 8. Top 10% vs Bottom 10% Analysis

Students were divided according to their Exam Score:

- **Top 10%:** Students at or above the 90th percentile.
- **Bottom 10%:** Students at or below the 10th percentile.

Their academic and behavioral characteristics were compared using tables and visualizations.

---

## 📈 Visualizations

The project includes:

- Exam Score distribution
- Hours Studied distribution
- Study Hours vs Exam Score scatter plot
- Attendance vs Exam Score scatter plot
- Previous Scores vs Exam Score scatter plot
- Sleep Hours vs Exam Score scatter plot
- Tutoring Sessions vs Exam Score scatter plot
- Physical Activity vs Exam Score scatter plot
- Correlation heatmap
- Top 10% vs Bottom 10% comparison chart

Regression lines are also used in relationship analysis to visually identify trends.

---

## 🧪 Hypothesis Testing

For selected variables, the following hypotheses were considered.

### Null Hypothesis (H₀)

There is no statistically significant linear relationship between the selected factor and Exam Score.

### Alternative Hypothesis (H₁)

There is a statistically significant linear relationship between the selected factor and Exam Score.

Pearson correlation and p-values were used to evaluate these hypotheses.

---

## 🔍 Top 10% vs Bottom 10%

The analysis compares high-performing and low-performing students across factors such as:

- Hours Studied
- Attendance
- Sleep Hours
- Previous Scores
- Tutoring Sessions
- Physical Activity
- Exam Score

This comparison helps identify behavioral and academic differences between the two groups.

---

## 💡 Key Insights

The analysis helps identify:

- Which factors show stronger associations with Exam Score.
- Which factors show weaker relationships.
- Differences between high-performing and low-performing students.
- Potential anomalies in the dataset.
- Whether observed relationships are statistically significant.

The exact numerical findings and correlations are generated directly from the dataset in the Google Colab notebook.

---

## ⚠️ Important Limitation

This project is an **Exploratory Data Analysis** and identifies associations between variables.

A correlation or statistically significant relationship **does not prove causation**.

Therefore, the findings should be interpreted as patterns and associations observed within the dataset rather than proof that one factor directly causes a change in examination performance.

---

## 📁 Project Files

```text
Student-Academic-Performance-EDA/
│
├── Student_Performance_EDA.ipynb
├── README.md
└── StudentPerformanceFactors.csv

# Student Performance Regression Analysis

## Project Overview

This project analyzes the relationship between students' weekly study hours and their Grade Point Average (GPA).

The goal was to determine whether study time is associated with academic performance and whether GPA can be predicted using study hours alone. The project includes exploratory data analysis, group comparison, statistical testing, correlation analysis, and a simple linear regression model.

The analysis focuses not only on building a model, but also on interpreting its results and understanding its limitations.

---

## Dataset

The dataset contains student-level observations with two main variables:

| Variable | Description |
|---|---|
| `gpa` | Student's Grade Point Average |
| `study_hours` | Number of weekly study hours |

The dataset contains **193 observations** and no missing values after initial inspection.

---

## Business / Analytical Questions

This project aims to answer the following questions:

- Do students who study more hours achieve higher GPA?
- Is the relationship between study hours and GPA statistically significant?
- Are there meaningful GPA differences between students who study less and those who study more?
- Can GPA be predicted using study hours alone?
- How well does a simple linear regression model explain academic performance?

---

## Tools and Libraries

The analysis was performed in Python using:

- `pandas` – data manipulation and analysis
- `numpy` – numerical operations
- `matplotlib` – data visualization
- `seaborn` – correlation visualization
- `scipy` – statistical testing
- `scikit-learn` – linear regression and model evaluation

---

## Analysis Workflow

The project follows a structured analytical workflow:

1. Data loading and initial inspection
2. Data cleaning
3. Exploratory Data Analysis (EDA)
4. Distribution analysis of GPA and study hours
5. Outlier inspection using boxplots
6. Study group comparison
7. Welch's t-test
8. Pearson correlation analysis
9. Linear regression modeling
10. Model evaluation
11. Actual vs predicted comparison
12. Residual analysis
13. Final conclusions

---

## Key Findings

### 1. GPA Distribution

Most students achieved GPA values between approximately **3.3 and 4.0**, suggesting generally good academic performance within the analyzed sample.

The GPA distribution was relatively concentrated, meaning that students' results did not vary extremely across the dataset.

---

### 2. Study Hours Distribution

Most students studied between **5 and 20 hours per week**.

The distribution of study hours was right-skewed, meaning that only a small number of students reported very high study time.

---

### 3. Study Group Comparison

Students were divided into two groups based on the median number of study hours:

- **Low Study** – students studying below the median
- **High Study** – students studying at or above the median

The High Study group achieved a slightly higher average GPA than the Low Study group. However, the difference was small.

Welch's t-test did not show a statistically significant difference between the two groups at the 0.05 significance level.

This suggests that study time alone does not strongly explain differences in GPA.

---

### 4. Correlation Analysis

Pearson correlation was used to measure the linear relationship between study hours and GPA.

The correlation coefficient was approximately:

```text
r = 0.133

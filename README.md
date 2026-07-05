# Correlation Analysis and Linear Regression

## Project Overview

This project analyzes the relationship between students' weekly study hours and their Grade Point Average (GPA).

The main goal is to determine whether the number of study hours is associated with academic performance and whether GPA can be predicted using study hours alone. The project combines exploratory data analysis, statistical testing, correlation analysis, and linear regression modeling.

---

## Dataset

The dataset contains student-level observations with information about GPA and weekly study hours.

### Variables

| Variable | Description |
|---|---|
| `gpa` | Student's Grade Point Average |
| `study_hours` | Number of weekly study hours |

The dataset contains **193 observations** and no missing values after initial inspection.

---

## Research Questions

This project aims to answer the following questions:

- Does studying more hours lead to higher GPA?
- Is the relationship between study hours and GPA statistically significant?
- Do students who study more achieve different GPA results than students who study less?
- Can GPA be predicted using study hours alone?
- How accurately does a simple linear regression model estimate students' GPA?

---

## Tools and Technologies

The project was created using Python and the following libraries:

- `pandas` – data manipulation and analysis
- `numpy` – numerical operations
- `matplotlib` – data visualization
- `seaborn` – correlation heatmap
- `scipy` – statistical testing
- `scikit-learn` – linear regression and model evaluation

---

## Analysis Workflow

The analysis follows a structured data analysis workflow:

1. Dataset loading and initial inspection
2. Data cleaning
3. Exploratory Data Analysis (EDA)
4. GPA and study hours distribution analysis
5. Outlier inspection using boxplots
6. Comparison of study groups
7. Welch's t-test
8. Pearson correlation analysis
9. Linear regression modeling
10. Model evaluation
11. Residual analysis
12. Final conclusions

---

## Key Results

### Exploratory Data Analysis

Most students achieved GPA values between approximately **3.3 and 4.0**, indicating generally good academic performance within the analyzed sample.

Study hours were positively skewed. Most students studied between **5 and 20 hours per week**, while only a small number of students reported very high study time.

### Study Group Comparison

Students were divided into two groups based on the median number of study hours:

- **Low Study**
- **High Study**

The High Study group had a slightly higher average GPA than the Low Study group. However, the difference was small.

Welch's t-test returned a p-value greater than 0.05, meaning that there was no statistically significant difference in GPA between the two study groups.

### Correlation Analysis

The Pearson correlation coefficient between study hours and GPA was approximately:

```text
r = 0.133

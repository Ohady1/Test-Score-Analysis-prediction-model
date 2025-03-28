Test Score Analysis Report

Project Overview:
This project analyzes students test scores in math, reading, and writing, examining the relationship between scores and various factors. The goal is to identify patterns and potential influences on student performance.

Dataset:
The dataset contains student test scores along with attributes such as:

Gender
Race/Ethnicity
Parental Level of Education
Lunch Type (Standard or Reduced Price)
Test Preparation Course (Completed or Not Completed)
Math Score
Reading Score
Writing Score

Exploratory Data Analysis (EDA):

Distribution of scores using histograms.
Relationship between scores and categorical attributes using bar plots.
Boxplots to examine score variability across different conditions.

Feature Engineering:

Created a new variable condition_count based on the presence of favorable factors:
Belonging to Race/Ethnicity Group E
Parental education at a Master's level
Standard lunch
Completion of a test preparation course

This variables were used as a target for predictions.

Predictive Modeling:
Linear Regression:

Used to predict condition_count from the three test scores.
Achieved 54.6% exact accuracy.

When allowing a +-1 range, accuracy increased to 95%, but this was considered too lenient.

Findings

Higher condition_count generally correlated with higher test scores.
Students who completed a test preparation course performed better on average.
Logistic Regression provided better category balance than Linear Regression.
The model struggled with predicting exact condition_count values but performed reasonably well with close predictions.

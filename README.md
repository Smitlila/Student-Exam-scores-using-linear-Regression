# Predicting Student Exam Scores using Linear Regression

## Overview
This project uses linear regression to predict students' final exam scores based on their weekly study hours and class attendance percentage. The goal is to explore how these variables affect student performance and evaluate the prediction accuracy of the model.

## Dataset
The dataset used for this project is sourced from Kaggle:
- **Dataset:** [Students Grading Dataset](https://www.kaggle.com/datasets/mahmoudelhemaly/students-grading-dataset)
- **Features:**
  - `Study_Hours_per_Week`
  - `Attendance (%)`
- **Target:**
  - `Final_Score`

## Steps and Techniques
- **Exploratory Data Analysis (EDA)**:
  - Visualized relationships using scatter plots.
  - Conducted descriptive statistics to understand data distribution.
- **Data Cleaning**:
  - Handled missing values by removing incomplete records:
    ```python
    data.dropna(subset=['Study_Hours_per_Week', 'Attendance (%)', 'Final_Score'], inplace=True)
    ```
- **Modeling**:
  - Split dataset into training (80%) and testing (20%) subsets.
  - Trained a linear regression model.
- **Evaluation**:
  - Used Mean Squared Error (MSE) to assess model performance.
- **Visualization**:
  - Scatter plot with regression line for study hours.
  - Bar chart comparing actual versus predicted final scores.

## Results
The model achieved a reasonable MSE, indicating effectiveness in predicting student performance based on study habits and attendance.

## Future Improvements
- Consider additional predictive variables (e.g., midterm scores, class participation).
- Apply advanced modeling techniques for enhanced prediction accuracy.

## Requirements
- Python libraries: pandas, numpy, matplotlib, seaborn, scikit-learn, kagglehub

## Usage
Run the notebook sequentially to replicate the analysis.

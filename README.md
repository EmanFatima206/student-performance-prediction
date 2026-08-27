# Student Performance Prediction

A machine learning project that predicts students' writing scores based on academic and demographic factors such as math score, reading score, parental education, lunch type, gender, and test preparation course.

## Project Overview

The goal of this project is to explore how machine learning can be used to predict student performance.

The project uses the Students Performance dataset and builds regression models to predict a student's writing score based on other available features.

The project also compares multiple machine learning algorithms and evaluates their performance using Mean Absolute Error (MAE) and R² score.

## Objective

The main objective of this project is to:

- Predict students' writing scores using machine learning.
- Preprocess categorical and numerical data.
- Compare different regression algorithms.
- Evaluate model performance using MAE and R².
- Visualize actual and predicted writing scores.
- Evaluate model performance using cross-validation.

## Dataset

The project uses the **Students Performance** dataset.

The dataset contains information about:

- Gender
- Race/Ethnicity
- Parental Level of Education
- Lunch
- Test Preparation Course
- Math Score
- Reading Score
- Writing Score

The **writing score** is used as the target variable.

## Technologies and Libraries

The project was developed using Python and Google Colab.

Main libraries used:

- Python
- Pandas
- Scikit-learn
- Matplotlib

## Data Preprocessing

Categorical variables were converted into numerical representations using one-hot encoding.

A preprocessing pipeline was also implemented to organize the preprocessing and model training steps.

The dataset was divided into training and testing sets using an 80/20 split.

A fixed `random_state=42` was used to make the train-test split reproducible.

## Machine Learning Models

Three regression models were trained and compared:

1. Linear Regression
2. Decision Tree Regressor
3. Random Forest Regressor

## Model Evaluation

Two evaluation metrics were used:

### Mean Absolute Error (MAE)

MAE measures the average absolute difference between the actual and predicted values.

A lower MAE indicates better performance.

### R² Score

R² measures how well the model explains the variation in the target variable.

A higher R² indicates better performance.

## Results

The models were evaluated on the test dataset.

| Model | MAE | R² |
|---|---:|---:|
| Linear Regression | 3.20 | 0.938 |
| Decision Tree | 4.54 | 0.862 |
| Random Forest | 3.69 | 0.915 |

Based on these results, Linear Regression performed best among the three evaluated models on the test set.

It achieved the lowest MAE and the highest R² score.

## Actual vs Predicted Visualization

An actual-vs-predicted scatter plot was created to visually compare the predicted writing scores with the actual writing scores.

Predictions closer to the diagonal reference line indicate better agreement between predicted and actual values.

## Cross-Validation

Five-fold cross-validation was also performed to evaluate whether the model's performance remained reasonably consistent across different subsets of the dataset.

This provides a more robust evaluation than relying only on a single train-test split.

## Project Workflow

```text
Dataset
   ↓
Data Loading
   ↓
Data Preprocessing
   ↓
One-Hot Encoding
   ↓
Train-Test Split
   ↓
Model Training
   ↓
Model Comparison
   ↓
MAE & R² Evaluation
   ↓
Actual vs Predicted Visualization
   ↓
Cross-Validation

## How to Run

### Google Colab

1. Open the Jupyter Notebook.
2. Upload the `StudentsPerformance.csv` dataset when prompted.
3. Run the notebook cells sequentially.






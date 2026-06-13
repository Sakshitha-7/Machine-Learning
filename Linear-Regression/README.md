# Medical Insurance Charges Prediction using Multiple Linear Regression

A beginner-level Machine Learning project that predicts medical insurance charges using **Multiple Linear Regression**. This project focuses on understanding the effect of outliers on model performance and compares different regression techniques after preprocessing and feature engineering.

---

## PROJECT OVERVIEW

This project uses the **Medical Insurance Cost Dataset** to predict medical insurance charges based on demographic and health-related information.

The project demonstrates:

- Exploratory Data Analysis (EDA)
- Correlation Analysis
- Outlier Detection using IQR
- Log Transformation
- Label Encoding
- Multiple Linear Regression
- Ridge Regression
- Lasso Regression
- Hyperparameter Tuning using GridSearchCV
- Model Evaluation and Comparison

---

## DATASET

**Dataset:** Medical Insurance Cost Dataset

**Dataset Link:**

https://www.kaggle.com/datasets/mirichoi0218/insurance

### Features

- Age
- Sex
- BMI
- Children
- Smoker
- Region

### Target Variable

- Charges (Medical Insurance Cost)

### Dataset Information

- Total Samples: **1338**
- Total Features: **6**
- Missing Values: **None**

---

## WORKFLOW

1. Load the dataset using Pandas.

2. Perform Exploratory Data Analysis (EDA):
   - Check dataset information
   - Check missing values
   - Generate descriptive statistics
   - Visualize distributions

3. Analyze feature relationships:
   - Correlation Heatmap
   - Scatter Plots
   - Distribution Plots

4. Detect outliers using:
   - Interquartile Range (IQR)
   - Boxplots

5. Remove outliers from the dataset.

6. Apply Log Transformation to reduce skewness in the target variable.

7. Encode categorical variables:
   - Sex
   - Smoker
   - Region

8. Split the dataset into:
   - Training Set
   - Testing Set

9. Train and evaluate:
   - Multiple Linear Regression
   - Ridge Regression
   - Lasso Regression

10. Perform Hyperparameter Tuning using GridSearchCV.

11. Compare model performances using:
   - MAE (Mean Absolute Error)
   - MSE (Mean Squared Error)
   - R² Score

---

## EXPLORATORY DATA ANALYSIS

Performed:

- Dataset statistics using `describe()`
- Missing value analysis
- Correlation Heatmap
- Scatter Plot between BMI and Charges
- Boxplot for Outlier Detection
- Distribution Plots

### Key Observations

- Charges are highly right-skewed.
- Significant outliers exist in the `charges` column.
- Smoking status has a strong impact on insurance charges.
- Higher BMI values tend to increase insurance costs.

---

## OUTLIER HANDLING

Outliers were detected using the **Interquartile Range (IQR)** method.

### Steps Performed

1. Calculate Q1 and Q3
2. Compute IQR
3. Determine lower and upper bounds
4. Remove outliers
5. Apply Log Transformation
6. Verify the distribution after transformation

### Observation

The log transformation reduced skewness and made the target variable closer to a normal distribution.

---

## FEATURE ENGINEERING

Categorical variables were converted into numerical values using Label Encoding.

Encoded Features:

- Sex
- Smoker
- Region

---

## MODELS IMPLEMENTED

### 1. Multiple Linear Regression

- Train/Test Split
- Model Training
- Prediction on Test Data
- Performance Evaluation

---

### 2. Ridge Regression

- Regularized Linear Regression
- Hyperparameter Tuning using GridSearchCV
- Best Alpha Selection

---

### 3. Lasso Regression

- Feature Selection using L1 Regularization
- Hyperparameter Tuning using GridSearchCV
- Best Alpha Selection

---

## MODEL PERFORMANCE

### Multiple Linear Regression

| Metric | Value |
|-------|------:|
| MAE | 3784.71 |
| MSE | 64,109,627.43 |
| R² Score | 0.6592 |

---

### Ridge Regression

| Metric | Value |
|-------|------:|
| Best Alpha | 0.1 |
| MAE | 3781.00 |
| MSE | 63,917,359.98 |
| R² Score | 0.6593 |

---

### Lasso Regression

| Metric | Value |
|-------|------:|
| Best Alpha | 0.001 |
| MAE | 3751.37 |
| MSE | 62,603,447.58 |
| R² Score | 0.6600 |

---

## VISUALIZATIONS INCLUDED

- Correlation Heatmap
- BMI vs Charges Scatter Plot
- Charges Distribution Plot
- Charges Boxplot
- Log Transformed Charges Distribution
- Log Transformed Charges Boxplot

These visualizations help understand:

- Feature relationships
- Outlier distribution
- Data skewness
- Effect of log transformation

---

## IMPORTANT OBSERVATION

For this dataset, outliers are **not always noise**.

Higher insurance charges for smokers or individuals with high BMI represent real-world patterns rather than errors.

This project explores how removing outliers and applying log transformation affect model performance and prediction accuracy.

---

## TECHNOLOGIES USED

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-Learn

---

## KAGGLE NOTEBOOK

View the complete notebook here:

https://www.kaggle.com/code/sakshitham/mlinearregression-dealingwithoutliers

---

## AUTHOR

**SAKSHITHA**

- B.Tech Student
-  **17 May 2026**


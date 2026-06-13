# Spam Mail Detection using Logistic Regression

A beginner-level Machine Learning project that detects whether an SMS message is **Spam** or **Not Spam** using **Logistic Regression** and Natural Language Processing (NLP) techniques.

---

## PROJECT OVERVIEW

This project uses the **SMS Spam Collection Dataset** to classify text messages as:

- Spam (1)
- Not Spam / Ham (0)

The project demonstrates:

- Data Cleaning
- Exploratory Data Analysis (EDA)
- Text Preprocessing
- Feature Extraction using TF-IDF
- Logistic Regression
- Model Evaluation
- Testing with Custom Messages

The SMS Spam Collection dataset contains **5,574 SMS messages** labeled as either spam or ham (not spam), making it a popular benchmark dataset for text classification and spam detection tasks. :contentReference[oaicite:0]{index=0}

---

## DATASET

**Dataset:** SMS Spam Collection Dataset

### Dataset Link

https://www.kaggle.com/datasets/uciml/sms-spam-collection-dataset

### Dataset Information

- Total Samples: **5572**
- Target Classes:
  - Spam = 1
  - Not Spam (Ham) = 0

### Features

- Message Text
- Target Label

### Missing Values

- None

---

## WORKFLOW

1. Load the SMS Spam dataset.

2. Perform Data Cleaning:
   - Remove unnecessary columns
   - Rename columns
   - Remove duplicate records
   - Check missing values

3. Perform Exploratory Data Analysis (EDA):
   - Class distribution
   - Message length analysis
   - Word count analysis
   - Character count analysis
   - Correlation analysis

4. Apply Text Preprocessing:
   - Convert text to lowercase
   - Tokenization
   - Remove special characters
   - Remove punctuation
   - Remove stop words
   - Apply stemming

5. Convert text into numerical features using:
   - TF-IDF Vectorization

6. Split the dataset into:
   - Training Set
   - Testing Set

7. Train Logistic Regression model.

8. Evaluate the model using:
   - Accuracy Score
   - Precision Score
   - Recall Score
   - F1 Score
   - Classification Report
   - Confusion Matrix

9. Test the model using custom messages.

---

## EXPLORATORY DATA ANALYSIS

Performed:

- Spam vs Ham Distribution
- Message Length Analysis
- Character Count Analysis
- Word Count Analysis
- Correlation Heatmap
- Boxplots for Outlier Detection

### Key Observations

- The dataset is imbalanced.
- Most messages are **Not Spam**.
- Spam messages are generally shorter than non-spam messages.
- Number of characters and number of words are highly correlated.

---

## TEXT PREPROCESSING

The following preprocessing techniques were applied:

- Lowercase Conversion
- Tokenization
- Removal of Special Characters
- Removal of Punctuation
- Stopword Removal
- Stemming

### Example

**Original Message**

```text
Congratulations! You won a FREE ticket. Call now!!!
```

**After Preprocessing**

```text
congratul won free ticket call
```

---

## FEATURE EXTRACTION

Text data cannot be directly used by machine learning algorithms.

Therefore, **TF-IDF Vectorization** was used to convert text into numerical vectors.

### Advantages of TF-IDF

- Gives importance to meaningful words
- Reduces importance of frequently occurring words
- Improves text classification performance

---

## MODEL IMPLEMENTED

### Logistic Regression

The Logistic Regression model was trained on TF-IDF transformed text features.

The model predicts:

- **1 → Spam**
- **0 → Not Spam (Ham)**

---

## MODEL PERFORMANCE

| Metric | Value |
|-------|------:|
| Accuracy | **97.29%** |
| Precision | **86.01%** |
| Recall | **93.89%** |
| F1 Score | **89.78%** |

---

## CLASSIFICATION REPORT

| Class | Precision | Recall | F1 Score |
|------|-----------:|-------:|---------:|
| Not Spam (0) | 0.99 | 0.98 | 0.98 |
| Spam (1) | 0.86 | 0.94 | 0.90 |

### Overall Accuracy

**97.29%**

---

## SAMPLE PREDICTIONS

### Example 1

**Input**

```text
Congratulations! You have won ₹50,000.
Call now to claim your prize.
```

**Prediction**

```text
Spam
```

---

### Example 2

**Input**

```text
Hey, are we meeting tomorrow at 10 AM?
```

**Prediction**

```text
Not Spam
```

---

## VISUALIZATIONS INCLUDED

- Spam vs Ham Count Plot
- Character Count Distribution
- Word Count Distribution
- Correlation Heatmap
- Boxplots for Outlier Detection

These visualizations help understand:

- Dataset imbalance
- Message length patterns
- Feature relationships
- Spam characteristics

---

## IMPORTANT OBSERVATION

A high Accuracy Score does not always mean a better model, especially for imbalanced datasets.

In spam detection:

- Precision tells how many predicted spam messages are actually spam.
- Recall tells how many actual spam messages are detected.
- F1 Score balances both Precision and Recall.

Therefore, evaluating multiple metrics is essential for building a reliable spam classifier.

---

## TECHNOLOGIES USED

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- NLTK
- Scikit-Learn

---

## KAGGLE NOTEBOOK

View the complete notebook here:

https://www.kaggle.com/code/sakshitham/logisticregression-spam-mail-detection

---
## PROJECT DETAILS

| Attribute | Value |
|----------|------|
| Project Type | Logistic Regression |
| Domain | Natural Language Processing (NLP) |
| Dataset | SMS Spam Collection Dataset |
| Date Created | **22-05-2026** |
| Programming Language | Python |
| Notebook Platform | Kaggle |

---
## AUTHOR

**SAKSHITHA**

- B.Tech Student



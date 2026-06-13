# KNN Iris Flower Classification

A beginner-level Machine Learning mini project that uses the K-Nearest Neighbors (KNN) algorithm to classify Iris flowers into three species: Setosa, Versicolor, and Virginica.

## PROJECT OVERVIEW

This is a beginner-level Machine Learning project implementing the **K-Nearest Neighbors (KNN) Classification algorithm** using the Iris dataset.

The project demonstrates:

- Data preprocessing
- Feature scaling
- Selecting the optimal K value
- Cross-validation
- Visualization
- Predicting flower species

---

## DATASET

**Source:** `sklearn.datasets.load_iris` (built-in)

- Samples: **150**
- Features: **4**
  - Sepal Length (cm)
  - Sepal Width (cm)
  - Petal Length (cm)
  - Petal Width (cm)

**Target Classes:**

- Setosa = 0
- Versicolor = 1
- Virginica = 2

**Missing Values:** None

---

## WORKFLOW

1. Load Iris dataset
2. Convert dataset into DataFrame
3. Check for missing values
4. Split data into training and testing sets
5. Apply feature scaling using `StandardScaler`
6. Train KNN classifier
7. Find suitable K value:
   - Heuristic approach (`√N`)
   - Experimental approach using Cross Validation
8. Evaluate model accuracy
9. Plot Accuracy vs K values
10. Visualize Decision Boundaries
11. Test model using custom input values

---

## MODEL PERFORMANCE

| Metric | Value |
|-------|------:|
| Test Accuracy | **91.11%** |
| Best Cross Validation Accuracy | **98.10%** |
| Optimal K Value | **4** |

---

## VISUALIZATIONS INCLUDED

- Accuracy vs K values graph
- Decision Boundary visualization

These visualizations help understand:

- How the value of K affects model performance
- How KNN divides the feature space into different classification regions

---

## EXAMPLE PREDICTION

**Input**

```text
Sepal Length = 5.1
Sepal Width  = 3.5
Petal Length = 1.4
Petal Width  = 0.2
```

**Output**

```text
Setosa
```

---

## COLAB NOTEBOOK

🔗 Colab Link:

https://colab.research.google.com/drive/1CNgB-2D4EuIqOpaGCSzvYtmzNpoPtQ4n?usp=sharing

---

## AUTHOR

**SAKSHITHA**

- B.Tech Student
-25/05/2026

---


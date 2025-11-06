# Rock vs Mine Detection – Machine Learning Practice Project

This project uses **Machine Learning (Logistic Regression)** to classify sonar signals as either **rocks** or **mines (metal objects)** under water.
It’s a **beginner-friendly ML practice project** created to understand the complete process of building and testing a model with real-world data.

---

## Project Overview

* **Goal:** Predict whether a sonar signal is reflected from a rock or a mine
* **Algorithm Used:** Logistic Regression
* **Dataset:** Sonar Dataset (from the UCI Machine Learning Repository)
* **Language:** Python
* **Libraries Used:**

  * `pandas` – data handling and analysis
  * `numpy` – numerical computation
  * `scikit-learn` – model building, training, and evaluation

---

## Steps and Workflow

### 1. Data Exploration

* Displayed the first and last 5 rows using `head()` and `tail()`
* Checked dataset shape and structure using `shape`
* Used `describe()` for statistical summary
* Counted target classes (`Rock` vs `Mine`)
* Grouped by the last column to compute mean feature values for each class

### 2. Data Preparation

* Split features (`x`) and labels (`y`)
* Divided data into **training** (90%) and **testing** (10%) sets using `train_test_split`
* Stratified splitting to maintain class balance

### 3. Model Training

* Used `LogisticRegression()` from scikit-learn
* Trained the model with `x_train` and `y_train`

### 4. Model Evaluation

* Evaluated accuracy on both training and testing data
* Verified model performance using `accuracy_score`

### 5. Making Predictions

* Converted new input data into NumPy arrays
* Reshaped the data (`reshape(1, -1)`) to match model input format
* Predicted output (`Rock` or `Mine`)
* Displayed prediction probabilities using `predict_proba()`

---

## What I Learned

* Data analysis with Pandas and NumPy
* Data splitting and preprocessing for ML
* Understanding of Logistic Regression
* Model accuracy testing and probability interpretation
* How `.iloc`, `.describe()`, and `value_counts()` work in Pandas

---

## Future Improvements

* Add a user interface (CLI, GUI, or web app)
* Try other algorithms (SVM, Random Forest, etc.)
* Apply feature scaling for optimization
* Visualize data using Seaborn/Matplotlib

---

## Example Output

```
Accuracy on training data :  0.83
Accuracy on test data :  0.76
Prediction : ['R']
Prediction Probability : [[0.72, 0.28]]
```

---

### Author

**Aruna Madugeeth**
Machine Learning Practice Project | Python | Logistic Regression | Sonar Dataset

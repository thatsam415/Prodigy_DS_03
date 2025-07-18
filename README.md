# Decision Tree Classifier – Bank Marketing

A machine learning project that builds a **Decision Tree Classifier** to predict whether a customer will subscribe to a term deposit based on demographic and behavioral data. The model uses the **Bank Marketing dataset** from the UCI Machine Learning Repository.

---

## 📌 Project Overview

This project demonstrates the application of data preprocessing, visualization, and Decision Tree modeling techniques to classify client subscription behavior in a marketing campaign run by a Portuguese bank.

---

## 📁 Dataset Description

- **Source**: [UCI Bank Marketing Dataset](https://archive.ics.uci.edu/ml/datasets/bank+marketing)
- **Records**: 41,188 client records
- **Goal**: Predict the binary target variable `y` – whether a client subscribes to a term deposit

### 🧾 Features:

| Column          | Description                                        |
|------------------|----------------------------------------------------|
| `age`           | Age of the client                                  |
| `job`           | Type of job                                        |
| `marital`       | Marital status                                     |
| `education`     | Education level                                    |
| `default`       | Has credit in default?                             |
| `housing`       | Has a housing loan?                                |
| `loan`          | Has a personal loan?                               |
| `contact`       | Contact communication type                         |
| `month`         | Last contact month of the year                     |
| `day_of_week`   | Last contact day of the week                       |
| `duration`      | Last contact duration in seconds                   |
| `campaign`      | Number of contacts during this campaign            |
| `pdays`         | Days since last contact in previous campaign       |
| `previous`      | Number of contacts before this campaign            |
| `poutcome`      | Outcome of previous campaign                       |
| `emp.var.rate`  | Employment variation rate                          |
| `cons.price.idx`| Consumer price index                               |
| `cons.conf.idx` | Consumer confidence index                          |
| `euribor3m`     | Euribor 3 month rate                               |
| `nr.employed`   | Number of employees                                |
| `y`             | Target: has the client subscribed to a deposit?    |

---

## 🧪 Technologies Used

- Python
- Pandas, NumPy
- Seaborn, Matplotlib
- Scikit-learn (DecisionTreeClassifier)
- Jupyter Notebook

---

## 🔍 Project Workflow

### 1️⃣ Data Preprocessing
- Missing values handled
- Duplicate entries removed
- Label encoding for categorical features
- Outlier treatment (IQR method)

### 2️⃣ Exploratory Data Analysis (EDA)
- Univariate and Bivariate visualizations
- Categorical and numerical insights
- Correlation heatmap

### 3️⃣ Feature Engineering
- Dropped highly correlated features: `emp.var.rate`, `euribor3m`, `nr.employed`

### 4️⃣ Model Building
- Split into training and test sets
- Built Decision Tree classifiers using:
  - `Gini` index
  - `Entropy` criterion

### 5️⃣ Evaluation
- Accuracy, Confusion Matrix, and Classification Report
- Visual representation of the decision tree

---

## 📈 Results

| Criterion | Training Accuracy | Testing Accuracy |
|-----------|-------------------|------------------|
| Gini      | ~93.6%            | ~93.3%           |
| Entropy   | ~93.6%            | ~93.2%           |

---

## 🧾 Conclusion

- Both Gini and Entropy performed well.
- Gini showed slightly better performance in identifying true positives.
- Visual tree representation aids business understanding and interpretability.

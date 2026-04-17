
# 🌲 Random Forest Model on Breast Cancer Dataset

This project applies a **Random Forest algorithm** using Python in Jupyter Lab to analyze and predict values from a dataset containing breast cancer-related features.

---

## 📁 Dataset

* File used: `data (1).csv`
* The dataset contains multiple numerical and categorical features.
* **Target variable:** `concave points_mean`

---

## ⚙️ Project Workflow

The project follows these main steps:

### 1. Data Loading

* Load dataset using `pandas`

### 2. Data Preprocessing

* Handle missing values:

  * Numerical columns → filled with mean
  * Categorical columns → filled with mode
* Encode categorical variables using `LabelEncoder`

### 3. Feature Selection

* Input features: all columns except target
* Target: `concave points_mean`

### 4. Train-Test Split

* 80% training data
* 20% testing data

### 5. Model Selection

* Automatically determines:

  * **Regression** if target is continuous
  * **Classification** if target is categorical

### 6. Model Training

* Uses `RandomForestRegressor` or `RandomForestClassifier`

### 7. Evaluation

* Regression:

  * Mean Squared Error (MSE)
  * R² Score
* Classification:

  * Accuracy
  * Classification Report

### 8. Feature Importance

* Visualized using `matplotlib`

---

## 🧠 Model Used

* Random Forest (Ensemble Learning Method)
* Library: `sklearn.ensemble`

---

## 🛠️ Technologies

* Python 🐍
* Jupyter Lab
* pandas
* numpy
* scikit-learn
* matplotlib

---

## ▶️ How to Run

1. Clone the repository:

```bash
git clone https://github.com/InaShametaj/BreastCancerRandomForest.git
cd BreastCancerRandomForest
```

2. Install dependencies:

```bash
pip install pandas numpy scikit-learn matplotlib
```

3. Run Jupyter Lab:

```bash
jupyter lab
```

4. Open the notebook and run all cells.

---

## 📊 Output

* Model performance metrics printed in console
* Feature importance visualization displayed as a plot

---

## ⚠️ Notes

* The target variable `concave points_mean` is continuous → model runs as **regression**
* Missing value handling updated to avoid pandas chained assignment warnings

---

## 📌 Future Improvements

* Hyperparameter tuning (GridSearchCV)
* Cross-validation
* Model comparison (e.g., XGBoost, SVM)
* Better visualization dashboards

---

## 👤 Author

*Ina Shametaj

---

## 📄 License

This project is open-source and available under the MIT License.

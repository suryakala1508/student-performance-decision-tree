# 🎓Student Performance Prediction using Decision Tree Classifier

## 📘 Overview

This project predicts whether a student will **pass or fail** based on academic and social attributes using a **Decision Tree Classifier**.
It focuses on **interpretable machine learning** — understanding *why* a student performs well or poorly.

---

## 🧩 Dataset

**Source:** UCI Machine Learning Repository — Student Performance Dataset

* Contains attributes like study time, absences, family support, and grades (`G1`, `G2`, `G3`).
* Target variable: `G3` (final grade), converted into binary classes: **Pass (1)** or **Fail (0)**.

---

## ⚙️ Workflow

1. **Data Preprocessing**

   * Filled missing values (median/mode).
   * Label encoded categorical variables.
   * Split dataset into training/testing sets.

2. **Model Training**

   * Used `DecisionTreeClassifier()` from Scikit-learn.
   * Evaluated using accuracy, confusion matrix, and classification report.

3. **Hyperparameter Tuning**

   * Used **GridSearchCV** to optimize:

     * `max_depth`, `min_samples_split`, `min_samples_leaf`, and `criterion`.

4. **Visualization & Insights**

   * Plotted the decision tree structure and feature importance.
   * Found top predictors: `G2`, `studytime`, and `failures`.

---

## 📊 Results

| Metric       | Before Tuning                 | After Tuning |
| ------------ | ----------------------------- | ------------ |
| Accuracy     | ~82%                          | **~88–90%**  |
| Top Features | `G2`, `failures`, `studytime` | Same         |

**Key Insights:**

* Consistent study time and higher mid-term grades strongly predict success.
* Decision tree provides interpretability — ideal for educational analytics.

---

## 🧠 Tech Stack

* **Language:** Python
* **Libraries:** Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn

---

## 🧩 File Structure

```
student-performance-decision-tree/
│
├── student_performance.ipynb        # Jupyter Notebook
├── data/student-mat.csv             # Dataset
├── results/tree_visualization.png   # Decision tree plot
├── results/feature_importance.png   # Feature importance chart
└── README.md                        # Project description
```

---

## 🚀 How to Run

1. Clone this repository

   ```bash
   git clone https://github.com/<your-username>/student-performance-decision-tree.git
   cd student-performance-decision-tree
   ```
2. Install dependencies

   ```bash
   pip install -r requirements.txt
   ```
3. Run the notebook

   ```bash
   jupyter notebook student_performance.ipynb
   ```

---

## 📎 Future Improvements

* Try Random Forest or Gradient Boosting for better accuracy.
* Add SHAP or LIME for deeper model explainability.
* Build a web app using Streamlit for interactive predictions.

---

## 👩‍💻 Author

**[B.Suryakala]**
📍 Data Science Enthusiast | Machine Learning Learner


# Logistic Regression on Customer Churn Prediction

## 🎯 Problem Statement and Goal of Project

This project applies **logistic regression** to predict customer churn based on demographic and behavioral features. The primary goal is to develop a clean, interpretable classification model and to demonstrate the impact of **outlier removal** and **class balancing** on model performance.

---

## 🛠 Solution Approach

The solution includes a full machine learning pipeline:

1. **Data Loading**:

   * Read the dataset (`ChurnData.csv`) containing customer records.
2. **Feature Selection**:

   * Use variables like `tenure`, `age`, `income`, `employ`, etc.
3. **Outlier Removal**:

   * Applied **IQR filtering** to eliminate extreme data points.
4. **Class Balancing**:

   * Used **undersampling** to balance the dataset between churn and non-churn customers.
5. **Feature Scaling**:

   * Standardized the features using `StandardScaler`.
6. **Train-Test Split**:

   * Split data into 67% training and 33% testing.
7. **Modeling**:

   * Trained a `LogisticRegression` model with default hyperparameters.
8. **Evaluation**:

   * Evaluated using accuracy, and probability predictions (`predict_proba`).

---

## 🧰 Technologies & Libraries

* Python 3
* `pandas`, `numpy` – data preprocessing
* `scikit-learn` – model building, scaling, evaluation
* `matplotlib` – plotting (optional)

---

## 📁 Dataset Description

* **File:** `ChurnData.csv`
* **Target Variable:** `churn` (1 = churned, 0 = retained)
* **Features Used**:

  * `tenure`, `age`, `address`, `income`, `ed`, `employ`, `equip`

This dataset represents anonymized customer information relevant for churn prediction in a subscription service.

---

## ⚙️ Installation & Execution Guide

1. Clone the repository or download the `.ipynb` file.
2. Place the dataset `ChurnData.csv` in the working directory.
3. Install required dependencies:

   ```bash
   pip install numpy pandas matplotlib scikit-learn
   ```
4. Open and run the notebook:

   ```bash
   jupyter notebook "reg logestic.ipynb"
   ```

---

## 📊 Key Results / Performance

* **Outlier Filtering**: Reduced noise, improving model focus.
* **Balanced Dataset**: Ensured fair representation of both churned and retained customers.
* **Logistic Regression Model**:

  * Successfully trained and predicted binary churn values.
  * Probabilistic outputs allow further threshold tuning.

---

## 📸 Sample Outputs

* 🧹 Outlier removal applied using IQR method
* ⚖️ Balanced dataset using undersampling
* ✅ Accuracy of the model printed
* 📈 Probability scores printed using `predict_proba()`

---

## 📚 Additional Learnings / Reflections

* This project was primarily designed to **demonstrate the working mechanics** of logistic regression in classification tasks, **not to optimize for the highest possible accuracy**.
* The goal was to gain hands-on experience with:

  * Preprocessing steps like **outlier removal** and **class balancing**.
  * Training a **baseline interpretable model** using logistic regression.
  * Observing how feature scaling and dataset quality affect classifier behavior.
* This type of exploration is essential for building **intuition** about model behavior, especially when working with real-world, imperfect data.

---

## 👤 Author

## Mehran Asgari

**Email:** [imehranasgari@gmail.com](mailto:imehranasgari@gmail.com)
**GitHub:** [https://github.com/imehranasgari](https://github.com/imehranasgari)

---

## 📄 License

This project is licensed under the MIT License – see the `LICENSE` file for details.

---

> 💡 *Some interactive outputs (e.g., plots, widgets) may not display correctly on GitHub. If so, please view this notebook via [nbviewer.org](https://nbviewer.org) for full rendering.*

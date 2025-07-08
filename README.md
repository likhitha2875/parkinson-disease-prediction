# parkinson-disease-prediction

# **Parkinson’s Disease Prediction Using Machine Learning**

This project builds a **machine learning pipeline** to predict **Parkinson’s disease** using **vocal and biomedical features** with an ensemble learning approach, ensuring **high accuracy and robustness**.

---

# 📌 Project Overview

* **Objective:** Early prediction of Parkinson’s disease using patient vocal data (frequency, jitter, shimmer, etc.)
* **Dataset:** UCI Parkinson’s dataset with 195 voice recordings and 23 vocal/biomedical features.
* **Model:** Voting Classifier Ensemble (Random Forest, XGBoost, SVM).
* **Accuracy Achieved:** \~88% cross-validation accuracy.

---

# ⚙️ Features of the Project

✅ Outlier removal using **IQR**
✅ **Standardization** using StandardScaler
✅ **SMOTE** for class imbalance handling
✅ **RFE** (Recursive Feature Elimination) for top 10 feature selection
✅ Ensemble **Voting Classifier** for robust prediction
✅ **ROC Curve and Confusion Matrix** for evaluation
✅ Clean, step-wise workflow for educational and deployment purposes

---

## **🔹 Dataset**

* Columns include **frequency measures, jitter, shimmer, noise-to-harmonics ratio, RPDE, DFA, spread1, D2, PPE, etc.**
* **Target:** `status` (1 = Parkinson’s, 0 = Healthy)

---

## **🔹 Model Pipeline**

1. Load and explore dataset
2. Drop irrelevant columns (`name`)
3. Remove outliers using IQR
4. Scale features with StandardScaler
5. Handle class imbalance with SMOTE
6. Feature selection with RFE (top 10 impactful features)
7. Train Voting Classifier (Random Forest + XGBoost + SVM)
8. Evaluate using:

   * Accuracy
   * Classification report
   * Confusion matrix
   * ROC Curve & AUC

---

## **💡 Results**

* **Accuracy:** \~85-89% on test data
* **Cross-Validation Accuracy:** \~88%
* **ROC AUC:** \~0.89-0.92

This demonstrates the **effectiveness of using ensemble learning with data cleaning and feature selection in healthcare predictive modeling.**

---

## **🚀 How to Run**

1️⃣ Clone this repository:

```bash
git clone https://github.com/yourusername/parkinsons-prediction.git
cd parkinsons-prediction
```

2️⃣ Install dependencies:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn imbalanced-learn xgboost
```

3️⃣ Run the notebook in **Google Colab or Jupyter Notebook** to train, test, and visualize the model.

---

## **📈 Use Cases**

✅ Early Parkinson’s screening in healthcare
✅ Telemedicine applications for non-invasive detection
✅ Biomedical signal analysis
✅ Machine Learning portfolio project

<div align="center">

# 🩺 Breast Cancer Classification using K-Nearest Neighbors (KNN)

### Machine Learning Classification Project


**Breast Cancer Classification using the K-Nearest Neighbors (KNN) algorithm to predict whether a tumor is Malignant or Benign based on diagnostic measurements.**

</div>

---

# 📌 Project Information

| Field | Details |
|-------|---------|
| **Author** | Akshat Garg |
| **Registration Number** | 23BCE10641 |
| **Application Number** | IN26011052 |
| **Batch Number** | 1A |
| **Email ID** | akshat.23bce10641@vitbhopal.ac.in |

---

# 🎯 Objective

The objective of this project is to develop a **K-Nearest Neighbors (KNN)** classification model (**k = 5**) capable of accurately classifying breast tumors as:

- 🔴 **Malignant (M)**
- 🟢 **Benign (B)**

using diagnostic measurements from the Breast Cancer Wisconsin Diagnostic Dataset.

---

# 📂 Dataset

**Dataset Name**

Breast Cancer Wisconsin Diagnostic Dataset

**Source**

https://www.kaggle.com/datasets/uciml/breast-cancer-wisconsin-data

---

# 🛠 Libraries Used

- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- kaggle

---

# ⚙️ Methodology

## 📊 Data Understanding

- Loaded and explored the dataset.
- Identified numerical features and the target variable (`diagnosis`).
- Examined feature distributions and data types.

---

## 🧹 Data Preprocessing

- Removed unnecessary columns:
  - `id`
  - `Unnamed: 32`
- Encoded the target variable:
  - Malignant (M) → **1**
  - Benign (B) → **0**
- Split the dataset into:
  - **80% Training**
  - **20% Testing**
- Applied **StandardScaler** to normalize all features.

---

## 🤖 Model Development

A **K-Nearest Neighbors (KNN)** classifier was trained using:

- **Algorithm:** KNeighborsClassifier
- **Number of Neighbors (k):** 5

The model predicts the diagnosis based on the majority class among the five nearest neighbors in the feature space.

---

## 📈 Model Evaluation

The trained model was evaluated using:

- ✅ Accuracy
- ✅ Precision
- ✅ Recall
- ✅ F1-Score
- ✅ Confusion Matrix Heatmap

---

# 📊 Results

| Metric | Score |
|---------|-------|
| **Accuracy** | **95.61%** |
| **Precision** | **97.44%** |
| **Recall** | **90.48%** |
| **F1-Score** | **0.9383** |

---

# 📌 Conclusion

The **K-Nearest Neighbors (KNN)** classifier with **k = 5** successfully classified breast tumor samples with an impressive **95.61% accuracy**.

Feature scaling using **StandardScaler** played a crucial role in ensuring that all diagnostic features contributed equally to the distance calculations.

Although KNN performs exceptionally well on relatively small medical datasets, its primary limitation is increased memory usage and slower prediction time as the dataset size grows.

---

# 🚀 Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-Learn
- Jupyter Notebook

---

# 📁 Project Structure

```
Breast-Cancer-KNN/
│
├── Breast_Cancer_Classification.ipynb
├── data.csv
├── README.md
└── requirements.txt
```

---

<div align="center">

### ⭐ If you found this project helpful, consider giving it a star!

Made with ❤️ using Python & Scikit-Learn

</div>

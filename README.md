# 🎗️ Breast Cancer Classification using K-Nearest Neighbors (KNN)

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![scikit-learn](https://img.shields.io/badge/scikit--learn-v1.0%2B-orange)
![License](https://img.shields.io/badge/License-MIT-green)

---

## 📌 Author Details

* **Author:** SATWIK TELANG
* **Registration Number:** 23BAI11046
* **Application Number:** IN26011013
* **Batch Number:** 1A
* **Email:** [satwik.23bai11046@vitbhopal.ac.in](mailto:satwik.23bai11046@vitbhopal.ac.in)

---

## 🎯 Objective

The primary objective of this project is to build a **K-Nearest Neighbors (KNN)** classification model with $k=5$ to accurately classify breast tumors as **Malignant (M)** or **Benign (B)** based on diagnostic features extracted from digitized images of fine needle aspirates (FNA) of breast masses.

---

## 📂 Dataset Information

* **Dataset:** [Breast Cancer Wisconsin (Diagnostic) Data Set](https://www.kaggle.com/datasets/uciml/breast-cancer-wisconsin-data)
* **Target Variable:** `diagnosis`
  * `M` (Malignant) $\rightarrow$ Encoded as `1`
  * `B` (Benign) $\rightarrow$ Encoded as `0`

---

## 🛠️ Tech Stack & Libraries

* **Data Handling & Processing:** `pandas`, `numpy`
* **Data Visualization:** `matplotlib`, `seaborn`
* **Machine Learning:** `scikit-learn`
* **Dataset Management:** `kaggle`

---

## 🔬 Methodology

1. **Data Understanding:** Explored feature distributions, data types, and verified target label balance.
2. **Data Preprocessing:**
   * Dropped non-informative columns (`id` and `Unnamed: 32`).
   * Label-encoded target class (`M: 1`, `B: 0`).
   * Performed **80/20 train-test split** with stratified sampling to preserve original class ratios.
   * Standardized features using **`StandardScaler`** to eliminate feature scale dominance across Euclidean distance calculations.
3. **Model Development:** Trained a `KNeighborsClassifier` with $k = 5$ on scaled training data.
4. **Model Evaluation:** Analyzed performace using Confusion Matrix heatmaps, Accuracy, Precision, Recall, and F1-Score.

---

## 📊 Results & Performance

| Metric | Score |
| :--- | :--- |
| **Accuracy** | **95.61%** |
| **Precision** | **97.44%** |
| **Recall** | **90.48%** |
| **F1-Score** | **0.9383** |

---

## 🚀 Quick Start

```bash
# Clone the repository
git clone [https://github.com/your-username/breast-cancer-knn.git](https://github.com/your-username/breast-cancer-knn.git)

# Navigate to project folder
cd breast-cancer-knn

# Install required dependencies
pip install pandas numpy matplotlib seaborn scikit-learn kaggle
```

---

## Conclusion

* The KNN model ($k=5$) achieved a **95.61% classification accuracy**.
* Feature scaling via **`StandardScaler`** is critical for distance-based models like KNN; without normalization, high-magnitude features disproportionately dominate distance calculations.
* **Limitations:** While KNN is highly effective and non-parametric for smaller diagnostic datasets, its main trade-offs are higher memory usage during inference and slower query speeds as dataset size scales ($O(n \cdot d)$ complexity per prediction).

# Bitcoin-Transaction-Anomaly-Detection-using-Unsupervised-Machine-Learning
Built an unsupervised Machine Learning pipeline to detect anomalies in Bitcoin transactions by selecting 19 key features from 700. Used PCA, t-SNE for dimensionality reduction, Isolation Forest for anomaly detection, and K-Means/DBSCAN for clustering. Applied Hampel filter for noise correction and evaluated performance using Random Forest-derived silhouette scores.
---

## 🧠 Key Concepts

- **Unsupervised Learning**: No labeled data required.
- **Dimensionality Reduction**: Visualization and structure discovery.
- **Clustering & Isolation**: Identify anomalous transactions.
- **Feature Analysis**: Understand key drivers of anomalies.

---

## 🚀 Technologies & Libraries

- Python 3.x
- NumPy / Pandas
- Scikit-learn
- Matplotlib / Seaborn
- t-SNE / PCA
- Isolation Forest / DBSCAN / K-Means
- Hampel Filter for outlier preprocessing

---

## 📊 Pipeline Overview

### 1. 📂 Data Preprocessing

- Transaction data is cleaned and normalized.
- **Hampel filter** is applied to remove extreme outliers and reduce noise.

### 2. 🔻 Dimensionality Reduction

- **PCA** is used to reduce feature space while retaining variance.
- **t-SNE** helps in visualizing complex, high-dimensional patterns.

### 3. 📌 Clustering for Pattern Discovery

- **K-Means Clustering** for identifying common behavior groups.
- **DBSCAN** for density-based anomaly detection and noise separation.
- **Silhouette Score** is used to evaluate cluster quality.

### 4. 🚨 Outlier Detection

- **Isolation Forest** detects anomalous transactions by isolating rare patterns.

### 5. 📈 Feature Importance

- A **Random Forest** model ranks the most influential features post-clustering to help interpret anomaly causes (e.g., transaction value, frequency, mining difficulty, sentiment metrics).

---

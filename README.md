# Credit Card Fraud Detection Using Unsupervised Learning

## Project Overview

Fraudulent transactions are extremely rare in financial systems, making them difficult to identify using traditional machine learning approaches. In many real-world scenarios, fraud labels may be unavailable, delayed, or incomplete. This project implements an unsupervised fraud detection system that identifies suspicious credit card transactions without using fraud labels during model training.

The project utilizes clustering and anomaly detection techniques to detect potentially fraudulent transactions and compares their effectiveness.

---

## Objectives

* Understand the structure of the credit card transaction dataset.
* Perform Exploratory Data Analysis (EDA).
* Preprocess and scale transaction data.
* Apply K-Means Clustering for anomaly detection.
* Apply Isolation Forest for anomaly detection.
* Use PCA for dimensionality reduction and visualization.
* Compare the performance of multiple unsupervised learning approaches.
* Evaluate results using actual fraud labels for benchmarking purposes.

---

## Dataset

**Dataset:** Credit Card Fraud Detection Dataset

The dataset contains transactions made by European cardholders and includes:

* 284,807 transactions
* 492 fraudulent transactions
* Highly imbalanced class distribution
* Features V1–V28 generated using PCA
* Additional features:

  * Time
  * Amount
  * Class (used only for final evaluation)

---

## Technologies Used

* Python
* Google Colab / Jupyter Notebook
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn

---

## Machine Learning Techniques

### 1. Data Preprocessing

* Missing value inspection
* Feature scaling using StandardScaler
* Feature preparation for unsupervised learning

### 2. Principal Component Analysis (PCA)

PCA is used for:

* Dimensionality reduction
* Visualization of transaction patterns
* Improving computational efficiency

### 3. K-Means Clustering

K-Means groups similar transactions into clusters. Transactions that are significantly distant from cluster centroids are treated as potential anomalies.

### 4. Isolation Forest

Isolation Forest is an anomaly detection algorithm specifically designed to identify rare and unusual observations. It isolates anomalies using random partitioning and is highly effective for fraud detection tasks.

---

## Project Workflow

1. Load Dataset
2. Perform Exploratory Data Analysis
3. Scale Features
4. Apply PCA
5. Train K-Means Clustering Model
6. Detect Anomalies Using K-Means
7. Train Isolation Forest Model
8. Detect Anomalies Using Isolation Forest
9. Compare Results
10. Evaluate Using Fraud Labels
11. Generate Conclusions and Recommendations

---

## Evaluation Metrics

The following metrics are used to evaluate model performance:

* Confusion Matrix
* Precision
* Recall
* Number of Detected Anomalies

---

## Results

The project compares K-Means and Isolation Forest based on:

* Number of anomalies detected
* Precision score
* Recall score
* Practical suitability for fraud detection

Isolation Forest generally performs better because it is specifically designed for anomaly detection, while K-Means is primarily a clustering algorithm.

---

## Business Impact

Early detection of fraudulent transactions can help financial institutions:

* Reduce financial losses
* Improve customer trust
* Enhance transaction monitoring systems
* Support fraud investigation teams

The proposed system can be integrated as an initial fraud-screening mechanism to flag suspicious transactions for further review.

---

## Repository Structure

```text
Credit-Card-Fraud-Detection/
│
├── credit_card_fraud_detection.ipynb
├── README.md
├── creditcard.csv
└── images/
```

---

## Future Improvements

* DBSCAN-based anomaly detection
* Autoencoder-based fraud detection
* Real-time fraud monitoring systems
* Ensemble anomaly detection techniques
* Hyperparameter optimization

---

## Author

Nazrin Nissam

B.Tech CSE | VIT Vellore

---

## License

This project is created for academic and educational purposes.


# Anomaly Detection in SMTP Protocol Using Deep Autoencoders

## 📌 Project Overview

This project focuses on detecting anomalous and malicious network activities in SMTP (Simple Mail Transfer Protocol) traffic using a Deep Learning Autoencoder model.

The system is trained on the NSL-KDD dataset and learns the normal behavior of network traffic. Any significant deviation from the learned patterns is identified as an anomaly, helping detect cyberattacks and suspicious activities.

The project demonstrates the application of Machine Learning and Deep Learning techniques in Network Security and Intrusion Detection Systems (IDS).

---

## 🚀 Features

* Data Cleaning and Preprocessing
* Categorical Feature Encoding
* Outlier Detection and Removal using IQR
* Feature Normalization using StandardScaler
* Deep Autoencoder Architecture
* Early Stopping for Optimal Training
* Anomaly Detection using Reconstruction Error
* Performance Evaluation using:

  * Confusion Matrix
  * Precision
  * Recall
  * F1-Score
  * ROC-AUC Score
* Visualization of Training Performance

---

## 🛠️ Technologies Used

* Python
* NumPy
* Pandas
* Matplotlib
* Seaborn
* Scikit-Learn
* TensorFlow
* Keras
* Jupyter Notebook

---

## 📂 Dataset

The project uses the **NSL-KDD Dataset**, an improved version of the KDD Cup 1999 dataset widely used for intrusion detection research.

### Dataset Features Include

* Protocol Type
* Service
* Connection Duration
* Source Bytes
* Destination Bytes
* Error Rates
* Login Information
* Traffic Statistics
* Attack Labels

---

## 🔄 Project Workflow

### 1. Data Loading

* Load NSL-KDD training and testing datasets
* Assign feature names

### 2. Data Cleaning

* Remove duplicate records
* Handle missing values
* Verify dataset integrity

### 3. Data Preprocessing

* Convert attack labels into binary classes:

  * Normal → 0
  * Attack → 1
* Encode categorical features
* Prepare feature and target variables

### 4. Outlier Removal

* Apply Interquartile Range (IQR) method
* Remove extreme outlier samples

### 5. Data Normalization

* Standardize features using StandardScaler
* Improve model convergence

### 6. Train-Test Split

* Training Set
* Validation Set
* Test Set

### 7. Autoencoder Model

#### Encoder

* Dense Layer (32 neurons)
* Batch Normalization
* Dense Layer (16 neurons)
* Latent Space (8 neurons)

#### Decoder

* Dense Layer (16 neurons)
* Dense Layer (32 neurons)
* Output Layer

### 8. Model Training

* Optimizer: Adam
* Loss Function: Mean Squared Error (MSE)
* Early Stopping
* Maximum 50 Epochs

### 9. Anomaly Detection

* Calculate reconstruction error
* Identify anomalies using threshold values
* Classify traffic as Normal or Attack

### 10. Evaluation Metrics

* Precision Score
* Recall Score
* F1 Score
* ROC Curve
* AUC Score
* Confusion Matrix

---

## 📊 Expected Results

The trained Autoencoder learns normal SMTP traffic behavior and detects suspicious network activities based on reconstruction error.

### Key Benefits

* High Detection Capability
* Reduced False Positives
* Efficient Network Monitoring
* Enhanced Cybersecurity Protection

---

## 📁 Project Structure

```text
Anomaly-dertection-in-smtp-protocol-using-Deepautoencoders/
│
├── Anomaly detect in smtp.ipynb
├── README.md
├── requirements.txt
├── dataset/
│   ├── KDDTrain+.txt
│   └── KDDTest+.txt
│
└── results/
    ├── confusion_matrix.png
    ├── roc_curve.png
    └── training_history.png
```

## ⚙️ Installation

### Clone Repository

```bash
git clone https://github.com/RAJEGOWDAC024/Anomaly-dertection-in-smtp-protocol-using-Deepautoencoders.git
cd Anomaly-dertection-in-smtp-protocol-using-Deepautoencoders
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

### Run Notebook

```bash
jupyter notebook
```

Open:

```text
Anomaly detect in smtp.ipynb
```

---

## 🎯 Applications

* Intrusion Detection Systems (IDS)
* Cybersecurity Monitoring
* SMTP Traffic Analysis
* Threat Detection
* Network Security Research
* Enterprise Security Solutions

---

## 👨‍💻 Author

**Raje Gowda C**

GitHub: https://github.com/RAJEGOWDAC024

Repository: https://github.com/RAJEGOWDAC024/Anomaly-dertection-in-smtp-protocol-using-Deepautoencoders

LinkedIn: https://www.linkedin.com/in/raje-gowda-c-a4b56929a/

---

## ⭐ Support

If you found this project useful, please consider giving the repository a star on GitHub.

Your support helps improve and maintain the project.

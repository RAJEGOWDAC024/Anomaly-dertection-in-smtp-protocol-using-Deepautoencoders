# Anomaly-dertection-in-smtp-protocol-using-DeepAutoencoders
Anomaly Detection in SMTP Protocol Using DeepAutoencoders

📌 Project Overview

This project focuses on detecting anomalous and malicious network activities in SMTP (Simple Mail Transfer Protocol) traffic using a Deep Learning Autoencoder model. The system is trained on the NSL-KDD dataset and learns the normal behavior of network traffic. Any significant deviation from the learned patterns is identified as an anomaly, helping detect cyberattacks and suspicious activities.

The project demonstrates the application of Machine Learning and Deep Learning techniques in Network Security and Intrusion Detection Systems (IDS).

🚀 Features

1.Data Cleaning and Preprocessing
2.Categorical Feature Encoding
3.Outlier Detection and Removal using IQR
4.Feature Normalization using StandardScaler
5.Deep Autoencoder Architecture
6.Early Stopping for Optimal Training
7.Anomaly Detection using Reconstruction Error
8.Performance Evaluation using:
9.Confusion Matrix
10.Precision
11.Recall
12.F1-Score
13.ROC-AUC Score
14.Visualization of Training Performance

🛠️ Technologies Used

1.Python
2.NumPy
3.Pandas
4.Matplotlib
5.Seaborn
6.Scikit-Learn
7.TensorFlow
8.Keras
9.Jupyter Notebook

📂 Dataset

The project uses the NSL-KDD Dataset, an improved version of the KDD Cup 1999 dataset widely used for intrusion detection research.

Dataset Features Include:
1.Protocol Type
-Service
-Connection Duration
-Source Bytes
-Destination Bytes
-Error Rates
-Login Information
-Traffic Statistics
-Attack Labels

🔄 Project Workflow

1. Data Loading
-Load NSL-KDD training and testing datasets.
-Assign feature names.

2. Data Cleaning
-Remove duplicate records.
-Handle missing values.
-Verify dataset integrity.

3. Data Preprocessing
Convert attack labels into binary classes:
-Normal → 0
-Attack → 1
-Encode categorical features.
-Prepare feature and target variables.

4. Outlier Removal
-Apply Interquartile Range (IQR) method.
-Remove extreme outlier samples.

5. Data Normalization
-Standardize features using StandardScaler.
-Improve model convergence.

6. Train-Test Split
Split data into:
-Training Set
-Validation Set
-Test Set

7. Autoencoder Model

Encoder:
-Dense Layer (32 neurons)
-Batch Normalization
-Dense Layer (16 neurons)
-Latent Space (8 neurons)

Decoder:
-Dense Layer (16 neurons)
-Dense Layer (32 neurons)
-Output Layer

8. Model Training
-Optimizer: Adam
-Loss Function: Mean Squared Error (MSE)
-Early Stopping implemented
-50 Epochs Maximum

9. Anomaly Detection
->Calculate reconstruction error.
->Identify anomalies using threshold values.
->Classify traffic as Normal or Attack.

10. Evaluation
-Precision Score
-Recall Score
-F1 Score
-ROC Curve
-AUC Score
-Confusion Matrix

📊 Expected Results:

The trained Autoencoder learns normal SMTP traffic behavior and detects suspicious network activities based on reconstruction error.

Key benefits:
1.High detection capability
2.Reduced false positives
3.Efficient network monitoring
4.Enhanced cybersecurity protection

📁 Project Structure
Anomaly-Detection-SMTP/
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

⚙️ Installation

1.Clone Repository
git clone https://github.com/RAJEGOWDAC024/Anomaly-dertection-in-smtp-protocol-using-Deepautoencoders.git
cd Anomaly-dertection-in-smtp-protocol-using-Deepautoencoders

2.Install Dependencies
pip install -r requirements.txt

3.Run Notebook
jupyter notebook

4.Open:
Anomaly detect in smtp.ipynb

🎯 Applications

-Intrusion Detection Systems (IDS)
-Cybersecurity Monitoring
-SMTP Traffic Analysis
-Threat Detection
-Network Security Research
-Enterprise Security Solutions

Author: Raje Gowda C
GitHub: https://github.com/RAJEGOWDAC024/
Repository: Anomaly Detection in SMTP Protocol Using Deep Autoencoders
Linkedin: https://www.linkedin.com/in/raje-gowda-c-a4b56929a/

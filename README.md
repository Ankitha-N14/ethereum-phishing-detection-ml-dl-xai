# Ethereum Phishing Detection using ML, DL and Explainable AI

## Paper Status

Submitted to *Journal of Systems Architecture* (Under Review)

---

## Overview

This project presents a blockchain-based phishing detection framework for Ethereum transactions using Machine Learning (ML), Deep Learning (DL), and Explainable AI (XAI).

The system analyzes real-world Ethereum transaction data to identify phishing attacks by learning behavioral patterns from transactional and temporal features.

---

## Problem Statement

Phishing attacks in blockchain are irreversible and financially damaging, as malicious transactions cannot be undone.

This project aims to:

* Detect phishing transactions accurately
* Handle real-world imbalanced datasets
* Provide model interpretability using Explainable AI

---

## Tech Stack

* Python
* Scikit-learn
* Deep Learning (Feedforward Neural Network)
* SHAP (Explainable AI)
* Pandas
* NumPy

---

## Dataset and Features

The model is trained on Ethereum transaction data with features such as:

* Transaction Value
* Block Height
* Timestamp
* Temporal Features (hour, day, month, weekday)

Both balanced and imbalanced datasets are used for realistic evaluation.

---

## Methodology

### Data Preprocessing

* Removed irrelevant fields (wallet address, transaction hash)
* Handled missing values and duplicates
* Converted timestamps into structured datetime features

### Feature Engineering

* Extracted temporal features (hour, day, month)
* Combined transactional and behavioral features

### Models Used

Machine Learning Models:

* Decision Tree
* Random Forest
* Gradient Boosting
* Support Vector Machine (SVM)
* K-Nearest Neighbors (KNN)

Deep Learning Model:

* Feedforward Neural Network (ANN)

---

## Evaluation Metrics

* Accuracy
* Precision
* Recall
* F1-Score
* ROC-AUC

---

## Results

* Random Forest achieved approximately 94% accuracy and performed best among all models
* Ensemble models and deep learning performed better in imbalanced datasets
* Deep learning captured complex transaction patterns effectively

---

## Explainable AI (SHAP)

To improve transparency and interpretability:

* Applied SHAP (SHapley Additive Explanations)
* Identified transaction value and temporal features as key indicators of phishing

---

## Key Contributions

* Integrated ML, DL, and XAI into a single framework
* Evaluated models on both balanced and imbalanced datasets
* Provided interpretable predictions using SHAP
* Developed a scalable approach for blockchain fraud detection

---

## Limitations

* Does not include graph-based blockchain relationships
* No smart contract code analysis
* Dependent on labeled datasets

---

## Future Work

* Graph Neural Networks (GNNs) for transaction networks
* Real-time phishing detection systems
* Smart contract analysis integration
* Adaptive learning for evolving attacks

---

## Repository Structure

ethereum-phishing-detection
│
├── data/
├── notebooks/
├── models/
├── paper.pdf
└── README.md

---

## How to Run

pip install -r requirements.txt
python main.py

---

## Author

Ankitha Nambiar
Data Science Student
Interested in Machine Learning, AI, and Blockchain Security


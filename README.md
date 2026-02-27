# 🏥 Enterprise Pharmacovigilance Risk Intelligence System



Internship Project — TCS iON AIP-225



An end-to-end enterprise healthcare analytics system designed to analyze Adverse Drug Reaction (ADR) data, classify severity levels using machine learning, and generate executive-level risk insights through structured dashboards.

##📌 Table of Contents

About the Project

Problem Statement

Features

Architecture

Tech Stack

Project Structure

Model Performance

Tableau Dashboard

Getting Started

Author

📖 About the Project



This project was developed as part of the TCS iON Industry Project Programme (AIP-225).



Pharmacovigilance systems handle large volumes of adverse drug event reports. Without structured governance and predictive modeling, identifying high-risk safety signals becomes difficult and delayed.



This system integrates:

Data governance and validation

Severity standardization (Mild, Moderate, Severe, Critical)

Feature engineering on demographic and drug-level attributes

Machine learning-based severity prediction

Executive-level dashboard visualization



The objective is to transform raw ADR case records into structured, decision-ready risk intelligence.

🎯 Problem Statement



To design and implement an enterprise-grade pharmacovigilance analytics system capable of:

Ensuring structured data quality validation

Predicting ADR severity using machine learning

Identifying high-risk drug and demographic patterns

Supporting data-driven safety monitoring and signal detection

✨ Features

✅ Structured data cleaning and validation pipeline

✅ Severity classification modeling

✅ Multi-model comparison (Logistic Regression, Random Forest, Gradient Boosting)

🚀 Random Forest–based severity prediction

📊 Tableau dashboard for executive risk monitoring

📈 Feature importance analysis

🔎 Rule-based high-risk escalation logic

🏗 Architecture



ADR Dataset

↓

Data Cleaning & Governance Validation

↓

Feature Engineering

↓

Train-Test Split (80:20)

↓

Model Training (Random Forest)

↓

Model Evaluation

↓

Risk Intelligence Dashboard (Tableau Public)

🛠 Tech Stack



Machine Learning & Data Processing

Python

Pandas

NumPy

Scikit-learn

Matplotlib

Seaborn



Platform

Google Colab (Jupyter Notebook)



Visualization

Tableau Public

📂 Project Structure

Enterprise-Healthcare-Risk-Intelligence-System/
│
├── Risk_analysis.ipynb
├── README.md
└── screenshots/
    ├── severity_distribution.png
    ├── confusion_matrix.png
    ├── tableau_dashboard.png
📊 Model Performance



Final Model Selected: Random Forest Classifier



Hyperparameters:

n_estimators = 150

max_depth = 12

random_state = 42

🔎 Overall Performance

Accuracy: 78.2%

Macro Average F1-Score: 0.22

Weighted Average F1-Score: 0.69

📈 Classification Insights



The model demonstrates strong predictive performance for the dominant severity class (Class 1):

Precision (Class 1): 0.78

Recall (Class 1): 1.00

F1-Score (Class 1): 0.88



However, minority classes (0, 2, 3) show near-zero precision and recall due to significant class imbalance in the dataset.



Dataset distribution (Test Set Example):

Class 1: 15,639 samples

Class 0: 697 samples

Class 2: 815 samples

Class 3: 2,849 samples



This indicates that while overall accuracy is high, the model is biased toward the majority class.

⚠️ Observed Limitation



The dataset exhibits strong class imbalance, resulting in:

Majority class dominance

Poor minority-class detection

Inflated overall accuracy



In regulated healthcare environments, this limitation must be addressed before production deployment.

🚀 Improvement Scope



To enhance minority severity detection:

Class weighting during training

SMOTE (Synthetic Minority Oversampling)

Balanced Random Forest

Threshold tuning for high-risk escalation

Multi-class optimization strategies

📈 Tableau Dashboard



The interactive Tableau dashboard provides:

Severity distribution analysis

High-risk rate by drug

Risk trend across age groups

Predicted vs actual severity comparison



🔗 Tableau Public Link:

(Paste your link here)

▶ Getting Started

Clone the repository

Open Risk_analysis.ipynb in Google Colab

Upload the dataset

Run all cells sequentially



Google Colab Link:

(Paste your Colab link here)

👩‍💻 Author



Garima

TCS iON AIP-225 Intern

Enterprise Healthcare Risk Intelligence — Batch 01



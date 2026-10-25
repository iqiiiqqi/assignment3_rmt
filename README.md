# assignment3_rmt
Comparative study of machine learning algorithms and class-imbalance strategies for banking fraud detection on large transaction data, with SHAP explanations and an Apache Spark scalability analysis.

# Fraud Detection in Banking Transactions: ML Algorithms and Big Data Analysis

Course project for Research Methods and Tools, Astana IT University.
Authors: Zhaniya Askarkyzy, Sabina Saiyn.

## Overview
This repository contains the code for a controlled comparison of machine
learning algorithms for detecting fraudulent banking transactions. The study
addresses class imbalance, concept drift (chronological validation),
scalability (Apache Spark) and explainability (SHAP).

## Research questions
- RQ1: Which supervised algorithms detect fraud best on highly imbalanced data?
- RQ2: How do imbalance-handling strategies affect the precision-recall trade-off?
- RQ3: How do training time and inference latency scale in a distributed framework?
- RQ4: Can the decisions of the best model be explained per transaction?

## Data
- European credit card dataset (Kaggle, ODbL): 284,807 transactions, 492 frauds.
- PaySim synthetic mobile-money dataset (Kaggle, CC BY-SA 4.0): 6,362,620 transactions, 8,213 frauds.

Datasets are not included. Download them from Kaggle and place them in `data/`.

## Models and strategies
Logistic Regression, Random Forest, XGBoost, CatBoost, MLP, stacking ensemble
and Isolation Forest. Imbalance handling: class weights, random
under-sampling and SMOTE. Split: chronological 60/20/20.

## Setup
- Python 3.11, Apache Spark 3.5
- `pip install -r requirements.txt`
- Random seeds: 42-46 (planned)



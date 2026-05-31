# Student Welfare Text Classification System

## Overview
This project is a machine learning system that analyzes student messages and classifies them into urgency levels. It helps detect critical welfare situations such as mental health risks, abuse, academic stress, financial issues, and spam.

The system uses NLP techniques to understand text and predict the appropriate category.

---

## Features
- Text classification of student reports
- Urgency prediction (critical → spam)
- Real-time prediction system
- Message routing into categories
- Ready for database integration (SQLite planned)

---

## Dataset
The dataset contains 305 records with:

- `text` → Student message
- `category` → Type of issue (Mental Health, Abuse, etc.)
- `category_weight` → Importance score
- `urgency_score` → Numeric urgency (0–1)
- `priority_score` → Priority ranking (0–10)
- `label` → Target class

---

## Problem Type
Multi-class text classification

### Labels:
- critical
- high
- medium
- low
- neutral
- spam

---

## Model Pipeline
The model uses:

- TF-IDF Vectorization
- Linear Support Vector Classifier (LinearSVC)

---

## Installation
```bash
pip install pandas scikit-learn joblib# student-warefare

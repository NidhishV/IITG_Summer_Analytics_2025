# 🌿 NDVI-Based Land Cover Classification (Summer Analytics 2025 Hackathon)

This project was created as part of the **Summer Analytics 2025 Hackathon**, hosted by the **Consulting & Analytics Club** and **GeeksforGeeks (GFG)**.

## 🚀 Problem Statement
Classify land cover types (Water, Impervious, Farm, Forest, Grass, Orchard) using **NDVI (Normalized Difference Vegetation Index)** time-series data from satellite imagery, with additional OpenStreetMap labels. The challenge includes handling **noisy** and **incomplete** NDVI signals and building a model that generalizes to clean data.

## 📊 Dataset
- **27 NDVI Time Points** (e.g., 20150720_N): NDVI values across dates.
- **Target Column**: `class` — categorical land cover labels.
- **ID**: Unique identifier for each data sample.

## 🧠 Approach
- **Imputation**: Mean imputation for missing NDVI values due to cloud cover.
- **Feature Engineering**:
  - Summary statistics (mean, std, max, min)
  - Temporal pattern features
- **Model**: Multinomial Logistic Regression (scikit-learn)
  - Balanced class weights to manage class imbalance
- **Evaluation Metric**: Accuracy

## 📁 Files
- `sa_hackathon.ipynb` – Complete notebook with EDA, preprocessing, model training, and prediction.
- `submission.csv` – Final submission file in the required format (`ID,class`).

## 🏁 Results
- Designed to generalize beyond noisy training data.
- Public leaderboard performance evaluated using accuracy.

## 📦 Libraries Used
- Python, NumPy, pandas, scikit-learn, matplotlib

## 📌 Notes
- Only Logistic Regression was allowed.
- The public test set includes noise; private test set is clean for final evaluation.

## 🏆 Outcome
- All participants receive GFG discounts.
- Top performers win GFG Premium memberships.

---

# 🎬 Movie Rating Prediction Using Machine Learning

This project predicts IMDb ratings for Indian movies based on structured metadata like genre, year, director, actors, and duration.

---

## ✅ Objective

Build a machine learning regression model that estimates the IMDb rating of a movie using its attributes.

---

## 📊 Dataset

- 📦 Source: [IMDb Indian Movies Dataset](https://www.kaggle.com/datasets/adrianmcmahon/imdb-india-movies)
- 🎥 Size: ~15,000 Indian movies (after cleaning: ~7,900 rows)
- 📌 Features used:
  - `Genre`
  - `Year`
  - `Duration`
  - `Director`
  - `Actor 1`
  - `Votes`

---

## 🧹 Preprocessing Steps

- Removed rows with missing `Rating`
- Extracted year from text
- Converted `Votes` and `Duration` to numeric
- Simplified and one-hot encoded:
  - Genre (main category only)
  - Top 10 Directors → others grouped as "Other"
  - Top 10 Actors → others grouped as "Other"

---

## 🤖 Models Trained

| Model                | RMSE  | MAE  |
|---------------------|-------|------|
| Linear Regression    | 1.23  | 0.97 |
| Decision Tree Regressor | 1.54  | 1.16 |

✅ **Linear Regression** gave better performance with lower average error.

---

## 📈 Evaluation

- Used **RMSE** (Root Mean Squared Error) and **MAE** (Mean Absolute Error) to measure performance.
- Plotted Actual vs Predicted ratings.
- Visualized top 10 most important features using Decision Tree.

---

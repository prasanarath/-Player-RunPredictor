# -Player-RunPredictor using Linear Regression

This project predicts the number of runs a cricket player might score in a match based on historical performance data using a Linear Regression model.

## 📊 Project Overview

The goal of this project is to apply machine learning techniques to predict a player's future performance—specifically, the number of runs scored—based on features such as:

- Batting position
- Balls faced
- Number of 4s and 6s hit
- Strike rate

We use a CSV dataset of past batting performances and build a regression model to estimate future scores.

---

## 🧠 Technologies & Libraries Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib

---

## 📁 Dataset : ODI World Cup 2023 Complete Datase ( https://www.kaggle.com/datasets/enggbilalalikhan/odi-world-cup-2023-complete-dataset?resource=download-directory)

The dataset used is a CSV file containing player-wise match data with the following columns:

- `Batsman_Name`
- `Runs`
- `Batting_Position`
- `Balls`
- `4s`
- `6s`
- `Strike_Rate`

> Missing values in the `Strike_Rate` column are handled using mean imputation.

---

## 🔍 Model Details

- **Algorithm Used**: Linear Regression
- **Target Variable**: `Runs`
- **Features Used**:
  - Batting_Position
  - Balls
  - 4s
  - 6s
  - Strike_Rate

### Evaluation Metrics:
- **Mean Squared Error (MSE)**
- **R² Score**

---

## 📈 Results

The trained model provides a high R² score (close to 1), indicating good prediction accuracy. A scatter plot is used to visualize predicted runs vs actual runs.

---

## 📊 Visualization

A scatter plot was generated comparing **Actual Runs** and **Predicted Runs**:

```python
plt.scatter(y_test, y_pred)
plt.xlabel("Actual Runs")
plt.ylabel("Predicted Runs")
plt.title("Actual vs Predicted Runs")

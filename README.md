# Task 1: Student Score Prediction

## 📌 Description
This project aims to build a model to **predict students' exam scores** based on various factors such as study hours, sleep, participation, and other related features.

**Dataset:** [Student Performance Factors (Kaggle)](https://www.kaggle.com/datasets)

### Objectives:
1. Perform **data cleaning** and basic **EDA** (visualization) to understand the dataset.
2. Split the dataset into **training** and **testing** sets.
3. Train a **Linear Regression** model to estimate the final score.
4. Visualize predictions and evaluate model performance.
5. Explore a **Polynomial Regression** model and compare its performance.
6. Experiment with **different feature combinations** (adding/removing features).

---

## 🛠 Tools & Libraries
- **Python**
- **Pandas** – data manipulation
- **Matplotlib** – visualization
- **Scikit-learn** – modeling & evaluation

---

## 📊 Workflow
1. **Data Cleaning**
   - Removed missing values
   - Encoded categorical variables using `pd.get_dummies`
   - Scaled numerical features using `StandardScaler`

2. **EDA**
   - Checked correlations between features and target
   - Visualized distributions and relationships

3. **Modeling**
   - **Linear Regression** as a baseline model
   - **Polynomial Regression** (degree=2) for capturing non-linear patterns
   - Feature combination testing (removing `sleep` and `participation`)

4. **Evaluation Metrics**
   - **MAE**: Mean Absolute Error
   - **MSE**: Mean Squared Error
   - **R² Score**: Coefficient of Determination

---

## 📈 Results

| Model | MAE | MSE | R² Score |
|-------|-----|-----|----------|
| Linear Regression | 2.9548 | 18.2978 | 0.4882 |
| Polynomial Regression (deg=2) | 1.1916 | 3.9474 | 0.8896 |
| Linear Regression (Without sleep/participation) | 2.9464 | 18.2404 | 0.4898 |

---

## 📌 Insights
- **Polynomial Regression** significantly outperformed Linear Regression with an **R² of ~0.89** compared to ~0.49.
- Removing `sleep` and `participation` had almost no effect on model performance.
- Learning Curve analysis showed **no severe overfitting** for the polynomial model.

---

## 🚀 Bonus Work
- Implemented **Polynomial Regression** and achieved a large performance boost.
- Experimented with **feature selection** to analyze importance and impact.

---


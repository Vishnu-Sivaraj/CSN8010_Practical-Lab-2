# 🧪 Practical Lab 2: Multivariate Linear Regression, Non-Parametric Models, and Cross-Validation

## 📘 Overview

This lab explores multiple regression techniques to predict diabetes progression using the **Diabetes dataset**. We begin with univariate polynomial regression on BMI, then expand to multivariate models including decision trees, k-nearest neighbors (kNN), and logistic regression. Each model is evaluated using standard performance metrics and compared for generalization and interpretability.

---

## 📂 Structure

The lab is divided into two main parts:

### 🔹 Part 2: Univariate Polynomial Regression on BMI
- Trained polynomial models (degrees 0–5) using only the BMI feature
- Evaluated using R², MAE, and MAPE on train, validation, and test sets
- Plotted fitted curve and data points
- Extracted model equation and predicted progression for a sample BMI
- Counted trainable parameters and discussed model limitations

### 🔹 Part 3: Multivariate Models
- Used all features (or dropped based on EDA)
- Trained and compared:
  - Two polynomial models (degrees 2 and 3)
  - Two decision trees (depths 3 and 5)
  - Two kNN models (k=3 and k=7)
  - Two logistic regression models (L2 and no penalty)
- Selected best model based on validation R²
- Evaluated best model on test set
- Predicted progression for a sample BMI
- Discussed trainable parameters and model limitations

---

## 📊 Performance Metrics

Each model was evaluated using:

- **R² (Coefficient of Determination)**: Measures explained variance
- **MAE (Mean Absolute Error)**: Measures average prediction error
- **MAPE (Mean Absolute Percentage Error)**: Measures relative error

These metrics helped assess both accuracy and generalization across datasets.

---

## 🏆 Best Models

- **Part 2**: Polynomial Regression (Degree 5)
  - Validation R²: 0.35
  - Test R²: 0.267
  - Test MAE: 51.75

- **Part 3**: kNN Regression (k=7)
  - Validation R²: 0.359
  - Test R²: 0.478
  - Test MAE: 41.52

---

## 📈 Visuals

- Part 2 includes a plot of the fitted polynomial curve over BMI with train, validation, and test data points.
- Part 3 focuses on tabular comparison and test set evaluation.

---

## 🧠 Workshop Integration

Key insights from peer-reviewed workshops were incorporated:

- **Performance Metrics**: Importance of MAE and MAPE for regression; recall and ROC-AUC for classification framing
- **KNN**: Bias-variance tradeoff and sensitivity to feature scaling
- **Logistic Regression**: Value of interpretable coefficients and calibrated probabilities

---

## ⚠️ Limitations

- Small dataset (~442 samples)
- MAPE instability near zero targets
- Polynomial models prone to overfitting
- Logistic regression less suited for continuous targets
- No cross-validation applied (future improvement)

---

## 🔮 Future Work

- Add cross-validation for more robust evaluation
- Explore ensemble methods (Random Forest, Gradient Boosting)
- Frame classification tasks using ROC-AUC and recall for clinical screening

---

## 👨‍💻 Author

**Vishnu Sivaraj**  

---

## 📎 Dataset

- **Diabetes dataset** from `sklearn.datasets.load_diabetes()`

---

## 📦 Dependencies

- Python 3.x  
- scikit-learn  
- pandas  
- matplotlib  

---

## ✅ How to Run

1. Clone the repository or open the notebook in Jupyter
2. Run cells sequentially from Part 2 to Part 3
3. Review outputs, plots, and conclusions

---

## 📌 Notes

This lab emphasizes clarity, transparency, and professional documentation. All models are evaluated fairly, and conclusions are grounded in actual results — not assumptions.

# 🏠 House Price Prediction using Linear Regression

## 📌 Project Overview
This project focuses on building and evaluating a **Linear Regression model** to predict house prices using the California Housing dataset. It demonstrates a complete machine learning workflow including data analysis, model training, and performance evaluation.

---

## 📊 Dataset Information
- **Total Records:** 20,640  
- **Features:** 9 numerical features  

### 🔑 Features:
- MedInc (Median Income)  
- HouseAge  
- AveRooms  
- AveBedrms  
- Population  
- AveOccup  
- Latitude  
- Longitude  

### 🎯 Target Variable:
- **MedHouseVal** (Median House Value)

---

## 🔍 Exploratory Data Analysis (EDA)
- Dataset contains **no missing values**  
- **MedInc** shows strong positive correlation (~0.69) with house prices  
- **AveRooms & AveBedrms** are highly correlated (~0.85) → multicollinearity  
- **Latitude & Longitude** show strong negative correlation (~-0.92)  
- Target variable is **slightly right-skewed**  
- Outliers present in **Population & AveOccup**

---

## ⚙️ Model Details
- **Algorithm:** Linear Regression  
- **Train-Test Split:** 80% / 20%  
- **Scaling:** Not applied (baseline model)

---

## 📈 Model Performance

| Metric | Value |
|--------|------|
| MAE    | 0.533 |
| MSE    | 0.556 |
| RMSE   | 0.746 |
| R²     | 0.576 |

### 📌 Interpretation:
- Model explains **~57.6% variance**  
- Shows **moderate performance**  
- Residual patterns indicate **missing non-linear relationships**

---

## 📊 Visualizations
- Feature Correlation Heatmap  
- Target Distribution Histogram  
- Residual Plot  
- Actual vs Predicted Plot  

---

## ✅ Conclusion
Linear Regression provides a **good baseline model**, but struggles with:
- Non-linear relationships  
- Outliers  
- Complex feature interactions  

---

## 🚀 Future Improvements
- Apply **Feature Scaling (Standardization)**  
- Handle **Outliers**  
- Reduce **Multicollinearity**  
- Use advanced models:
  - Ridge Regression  
  - Lasso Regression  
  - Random Forest Regressor  
  - Gradient Boosting (XGBoost)  

---

## 🛠️ Tech Stack
- Python  
- NumPy  
- Pandas  
- Matplotlib / Seaborn  
- Scikit-learn  

---

## 📌 How to Run

```bash
git clone https://github.com/Prashant517/Build-Evaluate-a-Linear-Regression-Model.git
cd Build-Evaluate-a-Linear-Regression-Model
pip install -r requirements.txt
python main.py

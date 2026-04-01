# House Price Prediction using Linear & Regularized Regression 

## Project Overview
This project focuses on predicting house prices using Linear Regression and its regularized variants Ridge, Lasso and ElasticNet.

The goal is to understand how different regression techniques perform and how regularization helps in improving model generalization.

---

## Objectives
- Build a baseline Linear Regression model  
- Apply regularization techniques (Ridge, Lasso, ElasticNet)  
- Compare model performance using evaluation metrics  
- Analyze feature importance and relationships  
- Understand the impact of multicollinearity and overfitting  

---

## Dataset
- Source: California Housing Dataset (from sklearn)
- Features include:
  - Median Income (MedInc)
  - Average Rooms (AveRooms)
  - Location (Latitude, Longitude)
  - Population and House Age
- Target:
  - House Price (in $100,000s)

---

## Tools & Technologies
- Python  
- NumPy, Pandas  
- Matplotlib, Seaborn  
- Scikit-learn  

---

## Workflow
1. Data Loading and Exploration  
2. Correlation Analysis  
3. Data Visualization  
4. Train-Test Split  
5. Feature Scaling using StandardScaler  
6. Model Training:
   - Linear Regression  
   - Ridge Regression (L2)  
   - Lasso Regression (L1)  
   - ElasticNet (L1 + L2)  
7. Model Evaluation (R² Score, RMSE)  
8. Coefficient Analysis  
9. Residual Analysis  

---

## Model Performance

| Model            | Train R² | Test R² | RMSE |
|------------------|---------|--------|------|
| Linear Regression | 0.613   | 0.576  | 0.7  |
| Ridge Regression  | 0.613   | 0.576  | 0.7  |
| Lasso Regression  | 0.497   | 0.481  | 0.8  |
| ElasticNet        | 0.531   | 0.515  | 0.8  |

*Best Model:* Linear Regression / Ridge Regression

---

## Key Insights
- Median Income (MedInc) is the most influential feature  
- Linear and Ridge performed similarly, indicating low overfitting  
- Lasso reduced some coefficients to zero (feature selection)  
- ElasticNet provided a balance between stability and sparsity  
- Residuals were randomly distributed, indicating a good model fit  

---

## Assumptions of Linear Regression
- Linearity between features and target  
- Independence of observations  
- Constant variance (Homoscedasticity)  
- Normal distribution of residuals  
- Low multicollinearity  

---

## Conclusion
This project demonstrates how different regression models perform on the same dataset and highlights the importance of regularization in improving model performance and generalization.

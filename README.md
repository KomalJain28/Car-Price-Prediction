# Car-Price-Prediction
Project Overview

This project predicts car prices using various machine learning models. The dataset was preprocessed by handling missing values, encoding categorical features, and splitting into training and testing sets. Multiple regression techniques were applied to determine the most accurate model.

Data Preprocessing

Cleaned and preprocessed the dataset
Encoded categorical variables
Splitted data into 80% training and 20% testing

Models Applied & Performance

1. Linear Regression
Training MSE: 1,115,682,770
Testing MSE: 1,978,359,735
Issue: High multicollinearity detected

2. Polynomial Regression
Training MSE: 918,423,944
Testing MSE: 1.227 × 10^20 (Overfitting)
Issue: Poor generalization

3. Regularization Techniques (Lasso, Ridge, Elastic Net)
Lasso: Training MSE: 1,115,738,395 | Testing MSE: 1,978,273,412
Ridge: Training MSE: 1,154,087,931 | Testing MSE: 1,981,482,019
Elastic Net: Training MSE: 3,420,360,051 | Testing MSE: 3,207,782,197
Issue: No significant improvement

4. KNN Regressor
Training MSE: 551,961,314
Testing MSE: 1,468,731,072
Issue: Poor generalization

5. SVR
Training MSE: 4,064,607,063
Testing MSE: 3,803,909,642
Issue: High errors, poor performance

6. Decision Tree Regressor
Training MSE: 1,050,102,366
Testing MSE: 1,921,020,876
Issue: Overfitting

7. Random Forest Regressor
Training MSE: 532,262,451
Testing MSE: 1,596,980,027
Performance: Good generalization

8. XGBoost Regressor (Best Model)
Training MSE: 560,266,121
Testing MSE: 1,568,032,996
Performance: Best balance between accuracy and generalization

Conclusion
Best Model: XGBoost Regressor (Lowest testing error, best generalization)
Alternative Model: Random Forest Regressor (Similar performance)
Polynomial regression overfitted, while KNN and SVR performed poorly

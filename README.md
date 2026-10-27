# Advanced_Regression_HousePrice_Dataset
# House Price Prediction Using Machine Learning

## 1. Project Overview

This project focuses on predicting house prices using different Machine Learning regression algorithms. The main objective is to compare multiple models, evaluate their performance, and identify a suitable model for predicting house prices.

The project explores regularization techniques, cross-validation strategies, tree-based regression models, and Support Vector Regression (SVR).

## 2. Project Objectives

- To understand regression algorithms in Machine Learning.
- To implement Ridge and Lasso Regression.
- To understand regularization and its effect on overfitting.
- To apply cross-validation techniques for model evaluation.
- To implement Decision Tree and Random Forest Regression.
- To evaluate Linear and RBF Support Vector Regression.
- To compare models using performance metrics.
- To analyze overfitting and underfitting.
- To identify a suitable model for house-price prediction.

## 3. Dataset Description

The project uses a house-price dataset containing property-related information.

The target variable used in the earlier implementation is:

- `house_price_inr` — the house price in Indian Rupees.

The identifier column is:

- `house_id` — a property identifier that is excluded from model training.

Other available property features are used as independent variables to predict house prices.

## 4. Technologies and Libraries Used

- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

## 5. Machine Learning Models

### Ridge Regression

Ridge Regression uses L2 regularization to reduce the magnitude of model coefficients and help control overfitting.

### Lasso Regression

Lasso Regression uses L1 regularization. It can reduce some coefficients to zero, helping with feature selection.

### Decision Tree Regression

Decision Tree Regression predicts house prices using feature-based decision rules. A tree that is too complex may overfit the training data.

### Random Forest Regression

Random Forest combines predictions from multiple decision trees. It can capture nonlinear relationships and often provides better generalization than a single decision tree.

### Support Vector Regression (SVR)

SVR predicts continuous values using a specified kernel. This project explores Linear SVR and RBF SVR.

## 6. Cross-Validation Techniques

The project discusses the following validation methods:

- **K-Fold Cross-Validation:** Divides the dataset into multiple folds for repeated training and validation.
- **Stratified K-Fold:** Preserves class proportions in classification. For regression, target values can be divided into bins to approximate stratification.
- **Leave-One-Out Cross-Validation (LOOCV):** Uses one observation for validation at a time.
- **Time Series Split:** Preserves chronological order when predicting future values from historical data.

The appropriate validation method depends on the dataset structure and prediction objective.

## 7. Model Evaluation Metrics

The models are evaluated using the following metrics:

- **MAE (Mean Absolute Error):** Measures the average absolute difference between actual and predicted prices.
- **MSE (Mean Squared Error):** Measures the average squared prediction error.
- **RMSE (Root Mean Squared Error):** Measures prediction error in the target variable's units.
- **R² Score:** Measures how well the model explains variation in house prices.

Generally, lower MAE and RMSE values and a higher R² score indicate better predictive performance when evaluated on the same test dataset.

## 8. Model Comparison

Based on the previously reported experimental results:

| Model | Reported R² Score |
|---|---:|
| Ridge Regression | 0.918840 |
| Decision Tree Regression | 0.853332 |
| Random Forest Regression | 0.927463 |
| Linear SVR | Negative |
| RBF SVR | Negative |

The exact Lasso score and the SVR scores were not provided in the reported results.

Random Forest achieved the highest reported R² score of 0.927463, followed by Ridge Regression with 0.918840.

These scores should be verified against the final notebook outputs before submission.

## 9. Overfitting and Underfitting

Overfitting occurs when a model performs very well on training data but performs poorly on unseen data.

Underfitting occurs when a model fails to learn the underlying patterns in both training and testing data.

Training and testing metrics can help identify these problems. Regularization, cross-validation, and appropriate hyperparameter tuning can help improve generalization.

## 10. How to Run the Project

1. Install Python and Jupyter Notebook.
2. Install the required Python libraries.
3. Place the house-price dataset in the appropriate project folder.
4. Open the Jupyter Notebook file.
5. Update the dataset path and target column if necessary.
6. Run the notebook cells in order.
7. Review model evaluation metrics and visualizations.
8. Compare model performance and write conclusions based on actual results.

Install the required libraries using:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn openpyxl jupyter
```

## 11. Conclusion

This project demonstrates the application of Machine Learning regression algorithms to house-price prediction.

The previously reported results indicate that Random Forest performed best among the tested models, followed by Ridge Regression. Regularization helps control model complexity, while cross-validation supports model selection and performance evaluation.

The project also highlights the importance of comparing training and testing performance to identify overfitting and underfitting.

Random Forest is a promising candidate for house-price prediction based on the reported results. Further validation using unseen and representative property data is recommended before real-world use.

## 12. Future Improvements

- Improve SVR performance through feature and target scaling.
- Perform systematic hyperparameter tuning.
- Add further exploratory data analysis and visualizations.
- Compare cross-validation results across models.
- Evaluate feature importance.
- Test the selected model on additional unseen data.


**Course/Class:** Add Your Course or Class

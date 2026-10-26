# forest-fire-weather-prediction
# Forest Fire Weather Prediction Using Machine Learning

## Overview

This project explores machine learning techniques using the Algerian Forest Fires dataset. It analyzes weather conditions associated with forest fires and develops models for fire-class classification and Fire Weather Index (FWI) regression.

## Objectives

- Clean and preprocess real-world environmental data.
- Perform exploratory data analysis and visualize patterns.
- Explore fire versus non-fire classification.
- Predict the continuous Fire Weather Index (FWI) using regression.
- Compare multiple regression algorithms using standard evaluation metrics.
- Save trained models for reuse.

## Technologies Used

- Python
- Pandas and NumPy
- Matplotlib and Seaborn
- Scikit-learn
- Joblib
- Google Colab

## Machine Learning Algorithms

- Random Forest Classifier
- Linear Regression
- Lasso Regression
- Ridge Regression
- ElasticNet
- LassoCV

## Model Evaluation

The regression models were evaluated using Mean Absolute Error (MAE), Root Mean Squared Error (RMSE), and R-squared (R²).

| Model | MAE | RMSE | R² |
|---|---:|---:|---:|
| Linear Regression | 0.4240 | 0.5962 | 0.9883 |
| LassoCV | 0.4398 | 0.6302 | 0.9869 |
| Tuned Lasso | 0.4483 | 0.6395 | 0.9865 |
| Lasso | 0.5481 | 0.7332 | 0.9823 |
| ElasticNet | 0.5253 | 0.8037 | 0.9787 |
| Ridge | 0.5685 | 0.8677 | 0.9752 |

Linear Regression achieved the best results among the evaluated regression models on the current test split, with an R² score of 0.9883.

These results are dataset- and split-specific and should be validated further before deployment.

## Skills Learned

- Data cleaning and missing-value handling
- Exploratory data analysis and data visualization
- Feature selection and leakage awareness
- Classification versus regression
- Feature scaling
- Model training and test-set evaluation
- Cross-validation and hyperparameter tuning
- Comparing models using MAE, RMSE and R²
- Saving and reusing models with Joblib and scikit-learn pipelines

## How to Run

1. Clone or download this repository.
2. Install the required libraries:

   `pip install pandas numpy matplotlib seaborn scikit-learn joblib openpyxl`

3. Open `forest_fire_analysis.ipynb` in Google Colab or Jupyter Notebook.
4. Place the dataset in the expected location and update the file path if needed.
5. Run the notebook cells in order.

## Limitations

This is an educational machine learning project. Predicting FWI is not the same as predicting the probability that a fire will occur. Performance on new locations and future weather data may differ.

## Future Improvements

- Validate preprocessing and scaling inside cross-validation pipelines.
- Perform residual analysis and more robust validation.
- Test generalization on separate regions or unseen data.
- Build a simple interface for making FWI predictions.

## Dataset

Add the original dataset source, attribution and applicable license here before publishing.

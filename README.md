# Car-Price-Prediction

This project focuses on building a regression model to predict the selling price of a used car based on its specifications like brand, fuel type, transmission, and ownership history.

# Dataset

Source: `CAR DETAILS FROM CAR DEKHO.csv`
The dataset contains the following columns:
- `name`: Name of the car (includes brand and model)
- `year`: Manufacturing year
- `selling_price`: Price the car was sold for
- `km_driven`: Kilometers driven
- `fuel`: Fuel type (Petrol, Diesel, etc.)
- `seller_type`: Type of seller (Dealer, Individual)
- `transmission`: Manual/Automatic
- `owner`: Ownership history

# Project Goals

1. Data Exploration
   Understand what features are available and how they impact the car price.

2. Feature Engineering
   - Dropped non-informative columns like car name.
   - Encoded categorical variables using `LabelEncoder`

4. Model Training & Selection
   - Used 2 regression models:
     - Random Forest Regressor
     - Gradient Boosting Regressor

5. Model Evaluation 
   - Evaluated models using:
     - MAE (Mean Absolute Error)
     - RMSE (Root Mean Squared Error)
   - Also performed 5-Fold Cross-Validation

# Libraries Used

- `pandas`, `numpy` - data handling
- `matplotlib`, `seaborn` - data visualization
- `scikit-learn` - machine learning models and metrics

# Results

------------------------------------------------------------------
| Model              | MAE                 | RMSE                |
|--------------------|---------------------|---------------------|
| Random Forest      | 169243.92989563596  | 393381.45215844986  |
| Gradient Boosting  | 174824.13205795066  | 396038.79143931455  |
------------------------------------------------------------------

# How to Run

1. Open the project in Google Colab or Jupyter Notebook
2. Upload the dataset: `CAR DETAILS FROM CAR DEKHO.csv`
3. Run the notebook cells step-by-step:
   - Data Cleaning
   - Exploratory Data Analysis (EDA)
   - Feature Engineering
   - Model Training & Evaluation
   - Cross-Validation

# Conclusion

- Newer cars tend to have higher resale prices  
- Brand has a strong influence on the dataset distribution  
- Random Forest and Gradient Boosting performed better than Linear Regression  
- Cross-validation gave more reliable performance estimation

# Car-Price-Prediction

This project predicts used car prices based on various features like brand, year, fuel type, transmission, etc. It uses regression models to help estimate a car's value using a dataset from CarDekho.

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
   - Removed duplicate rows  
   - Extracted brand from the `name` column  
   - Transformed `selling_price` using log scale  
   - Encoded categorical variables using `LabelEncoder`

3. Model Training & Selection
   - Used 3 regression models:
     - Linear Regression
     - Random Forest Regressor
     - Gradient Boosting Regressor
   - Split data into training (80%) and testing (20%) sets

4. Model Evaluation 
   - Evaluated models using:
     - MAE (Mean Absolute Error)
     - RMSE (Root Mean Squared Error)
   - Also performed 5-Fold Cross-Validation and printed average CV RMSE

# Libraries Used

- `pandas`, `numpy` - data handling
- `matplotlib`, `seaborn` - data visualization
- `scikit-learn` - machine learning models and metrics

# Results

------------------------------------------------------------------
| Model              | MAE                 | RMSE                |
|--------------------|---------------------|---------------------|
| Linear Regression  | 0.30153565129181176 | 0.3908131584349638  |
| Random Forest      | 0.317475005010856   | 0.4229418624351199  |
| Gradient Boosting  | 0.3633706671768348  | 0.47365417875512167 |
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

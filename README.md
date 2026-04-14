Objective

The goal of this project is to predict medical insurance charges based on personal attributes such as age, BMI, smoking status, and other demographic factors using a Linear Regression model.

 Approach

1. Data Preparation
Loaded the Medical Cost Personal Dataset
Separated:
Features (age, sex, bmi, children, smoker, region)
Target (charges)
Applied One-Hot Encoding to categorical variables:
sex
smoker
region

2. Model Building
Used a Linear Regression model
Built a pipeline combining:
Preprocessing (encoding categorical variables)
Model training

3. Training & Testing
Split data into:
80% Training
20% Testing
Trained the model on training data
Generated predictions on test data

4. Evaluation Metrics
Mean Absolute Error (MAE): 4181.19
Root Mean Squared Error (RMSE): 5796.28

These metrics indicate the average prediction error:

MAE shows average absolute deviation
RMSE penalizes larger errors more strongly

 Visualizations & Insights

1. BMI vs Charges
Weak to moderate positive relationship
Higher BMI tends to increase insurance costs, but with variability

2. Age vs Charges
Strong positive correlation
Older individuals generally have higher medical costs

3. Smoking vs Charges
Most significant factor
Smokers have dramatically higher insurance charges than non-smokers

Key Insights

 Smoking status is the strongest predictor of insurance cost
 Age is highly correlated with increased charges
 BMI has some influence, but less than smoking and age
 Number of children and region have relatively smaller effects

 Conclusion

The Linear Regression model provides a reasonable baseline for predicting insurance costs. However:
Performance can be improved using advanced models (e.g., Random Forest, Gradient Boosting)
Feature engineering and interaction terms (e.g., smoker × age) could enhance accuracy

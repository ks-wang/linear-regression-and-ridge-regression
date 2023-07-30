# House Price Prediction using Linear Regression and Ridge Regression

## Introduction:
This report explores a dataset containing house sale prices for King County, USA, which includes Seattle. The objective is to build regression models for predicting house prices based on various features. Both Linear Regression and Ridge Regression will be used to perform the predictions, and their performances will be evaluated. The dataset includes information such as the number of bedrooms, bathrooms, square footage of the home, waterfront view, and other relevant factors that may influence house prices.

## Analysis:

### Data Preprocessing:
The dataset was imported, and data wrangling was performed to handle missing values in the 'bedrooms' and 'bathrooms' columns. The 'id' and 'Unnamed: 0' columns were dropped as they were irrelevant to the analysis.

### Exploratory Data Analysis:
Exploratory data analysis was conducted to understand the distribution and correlation of various features with the target variable 'price.' It was identified that 'sqft_living' had the highest positive correlation with 'price' (R^2=0.49).

### Model Development:
Multiple regression models were built to predict house prices. Firstly, a Linear Regression model was fitted using 'sqft_living' as the feature, resulting in an R^2 value of 0.49. Next, several features such as 'floors,' 'waterfront,' 'bedrooms,' 'view,' and others were included to build a more complex model. This multiple regression model achieved an R^2 value of 0.66.

### Model Evaluation and Refinement:
The data was split into training and testing sets to evaluate the model performance using Ridge Regression. The Ridge model with regularization parameter = 0.1 achieved an R^2 of 0.65. Additionally, a second-order polynomial transform was performed on the features and fitted to the Ridge Regression model, resulting in an improved R^2 value of 0.70.

## Conclusion:
In this analysis, successful regression models were developed to predict house prices based on various features. The multiple regression model demonstrated a decent R^2 value of 0.66, indicating its ability to explain the variance in house prices. Furthermore, the Ridge Regression model with polynomial features achieved the best R^2 value of 0.70, demonstrating its superior predictive power compared to the other models.

Overall, this study provides valuable insights into the factors affecting house prices in King County, USA. Real estate professionals or potential buyers/sellers can use the developed models to estimate house prices more accurately.

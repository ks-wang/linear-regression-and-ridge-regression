# House Price Prediction using Linear Regression and Ridge Regression

## Introduction:
In this report, we explore the dataset containing house sale prices for King County, USA, which includes Seattle. Our objective is to build a regression model that can predict house prices based on various features. We will use both Linear Regression and Ridge Regression to perform the prediction and evaluate their performances. The dataset includes information such as the number of bedrooms, bathrooms, square footage of the home, waterfront view, and other relevant factors that may influence house prices.

## Analysis:

### Data Preprocessing:
We began by importing the dataset and performed data wrangling to handle missing values in the 'bedrooms' and 'bathrooms' columns. Then, we dropped the 'id' and 'Unnamed: 0' columns as they were not relevant for the analysis.

### Exploratory Data Analysis:
We conducted exploratory data analysis to understand the distribution and correlation of various features with the target variable 'price.' We identified that 'sqft_living' had the highest positive correlation with 'price' (R^2=0.49).

### Model Development:
We built multiple regression models to predict the house prices. Firstly, we used 'sqft_living' as the feature and fitted a Linear Regression model, resulting in an R^2 value of 0.49. Next, we included several features such as 'floors,' 'waterfront,' 'bedrooms,' 'view,' and others to build a more complex model. This multiple regression model achieved an R^2 value of 0.66.

### Model Evaluation and Refinement:
We split the data into training and testing sets to evaluate the model performance using Ridge Regression. The Ridge model with regularization parameter = 0.1 achieved an R^2 of 0.65. Additionally, we performed a second-order polynomial transform on the features and fitted the Ridge Regression model, resulting in an improved R^2 value of 0.70.

## Conclusion:
In this analysis, we successfully developed regression models to predict house prices based on various features. The multiple regression model demonstrated a decent R^2 value of 0.66, indicating its ability to explain the variance in house prices. Furthermore, the Ridge Regression model with polynomial features achieved the best R^2 value of 0.70, indicating its superior predictive power compared to the other models.

Overall, this study provides valuable insights into the factors affecting house prices in King County, USA. The developed models can be used by real estate professionals or potential buyers/sellers to estimate house prices more accurately. However, further improvements could be made by exploring other advanced regression techniques and incorporating additional features or domain-specific knowledge to enhance the model's performance.

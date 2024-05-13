# CA_house_price_prediction


1. Project Title: Predicting House Prices in California.

2. Project Overview:  This project aims to predict median house prices in California using machine learning techniques.

3. Dataset Source:  https://www.kaggle.com/datasets/harrywang/housing

4. Techniques Used: Linear Regression and Random Forest Regression.

5. Data Preprocessing:
During the data preprocessing stage, I ensured that the dataset was ready for analysis by performing the following steps:
a)Handling Missing Values: Any missing values in the dataset were removed to maintain the integrity of our analysis.
b)Handling Categorical Data: One of the columns, ocean_proximity, contained non-numeric values that couldn't be directly used in our machine learning models. To address this, I used the get_dummies() function in the Pandas library. This function converts categorical variables into dummy/indicator variables, effectively transforming them into a machine-readable format without needing to use one-hot encoding explicitly.
6.Feature Engineering:
In the feature engineering phase, I introduced additional features to enhance the predictive capabilities of our models:
  a)Bedroom Ratio: This feature represents the ratio of bedrooms to total rooms in each house. By calculating this ratio, we gain insight into the proportion of bedrooms relative to the overall size of the property.
  b)Household Rooms: Another new feature is household_rooms, which calculates the average number of rooms per household in a given area. This metric provides valuable information about the average household size, which could influence housing prices.
These engineered features aim to provide our machine learning models with more relevant information for accurately predicting house prices in California.


7. Model Implementation: For the implementation of machine learning models, the following steps were taken:
a)Data Splitting: The dataset was split into training and testing sets using Scikit-learn's train_test_split() function. This ensures that the model is trained on one subset of the data and evaluated on another subset to assess its performance.
b)Model Training: Two regression models were trained on the training data:
    * Linear Regression: Implemented using Scikit-learn's LinearRegression class.
    * Random Forest Regression: Utilized Scikit-learn's RandomForestRegressor class.
c)Model Evaluation: The trained models were evaluated using the testing data to assess their predictive performance. 
d)Performance Comparison: Finally, the performance of the two models was compared to determine which one provided better predictions for median house prices in California.


8. Results:  The Random Forest Regression model exhibited superior predictive accuracy with a test score of approximately 80%, surpassing the Linear Regression model, which achieved around 60% accuracy. This difference highlights the effectiveness of Random Forest Regression in accurately predicting median house prices in California.










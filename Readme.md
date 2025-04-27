# Predicting Housing Prices Using Machine Learning

## Overview

This project focuses on predicting house prices based on various features such as area, number of bedrooms, bathrooms, and amenities. We used several machine learning models including Linear Regression, Random Forest, Gradient Boosting, AdaBoost, Support Vector Regressor (SVR), and Decision Tree to predict the price of a house. After evaluating the performance of these models, Gradient Boosting emerged as the best performer, achieving an R² score of 0.67. The project also explores the significance of different features in determining house prices, highlighting the impact of area, number of bathrooms, and air conditioning.

## Key Features
- **Machine Learning Models**: Multiple models were applied, including Linear Regression, Random Forest, Gradient Boosting, AdaBoost, SVR, and Decision Tree.
- **Feature Importance**: The Gradient Boosting model revealed that area, number of bathrooms, and air conditioning were the most significant factors affecting house prices.
- **User Interface**: A user-friendly interface allows users to input house features and receive an estimated house price prediction.
- **Model Evaluation**: The Gradient Boosting model was found to provide the best performance with an R² score of 0.67.

## Dataset Overview

The dataset contains 13 features and 545 samples, with the target variable being the house price. The features include both numerical (e.g., area, bedrooms, bathrooms) and categorical data (e.g., presence of air conditioning, whether the house is on a main road). The dataset posed challenges due to multicollinearity among features, requiring advanced preprocessing and robust modeling techniques.

### Dataset Features:
- **Price**: Price of the house (target variable) [Numerical]
- **Area**: Total area of the house [Numerical]
- **Bedrooms**: Number of bedrooms in the house [Numerical]
- **Bathrooms**: Number of bathrooms in the house [Numerical]
- **Stories**: Number of stories in the house [Numerical]
- **Mainroad**: Proximity to the main road [Categorical]
- **Guestroom**: Availability of a guest room [Categorical]
- **Basement**: Presence of a basement [Categorical]
- **Hotwaterheating**: Presence of a hot water heating system [Categorical]
- **Airconditioning**: Presence of air conditioning [Categorical]
- **Parking**: Number of parking spaces available [Numerical]
- **Prefarea**: Preference for a specific area [Categorical]
- **Furnishingstatus**: Furnishing status [Categorical]

## Data Preprocessing

The preprocessing steps included:
1. **Categorical Encoding**: Applied One-Hot Encoding to convert categorical features into numerical format.
2. **Feature Scaling**: StandardScaler was used to normalize numerical features like area, bedrooms, and bathrooms.
3. **No Missing Data**: The dataset did not have missing values, simplifying preprocessing.

These steps ensured that the dataset was clean and ready for model training.

## Model Evaluation and Results

The models were evaluated using **Mean Squared Error (MSE)** and **R² scores**. The following are the results:

| Model                          | MSE (Mean Squared Error)      | R² Score |
|---------------------------------|-------------------------------|----------|
| Linear Regression               | 1,754,318,687,330.67          | 0.65     |
| Random Forest                   | 1,959,323,004,717.27          | 0.61     |
| Gradient Boosting               | 1,688,403,924,777.51          | 0.67     |
| AdaBoost                        | 2,237,444,322,297.88          | 0.56     |
| Support Vector Regressor (SVR)  | 5,567,929,077,615.07          | -0.10    |
| Decision Tree                   | 2,642,802,637,614.68          | 0.48     |

**Gradient Boosting** outperformed all other models, achieving the highest R² score (0.67) and the lowest MSE. The **Support Vector Regressor** and **Decision Tree** models performed poorly, with SVR showing a negative R² score, indicating it was ineffective for this dataset. **Linear Regression** was also competitive, with a R² score of 0.65.

### Feature Importance:
The Gradient Boosting model identified the following features as most significant:
- **Area**: 46.43%
- **Bathrooms**: 16.92%
- **Air Conditioning (Yes)**: 9.15%
- **Parking**: 4.86%
- **Stories**: 4.59%

These results highlight the importance of structural features (like area and number of bathrooms) and amenities (like air conditioning) in predicting house prices.

## Conclusion

This project successfully demonstrated the application of machine learning models for predicting housing prices. The **Gradient Boosting** model was the most effective, providing a strong R² score of 0.67. This project also emphasizes the importance of features like area and number of bathrooms in predicting house prices. 

A **user-friendly interface** was created, allowing users to input house features and receive price predictions. The model can be further improved by integrating more data and exploring deep learning techniques to enhance prediction accuracy. 


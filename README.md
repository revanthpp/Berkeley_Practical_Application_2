# Practical_Application_2

# What Drives the Price of a Car?

This project explores a dataset of used car listings to understand the factors that influence car prices.  The goal is to provide actionable recommendations to a used car dealership based on these findings.

## Programming Language and Libraries

This analysis was performed using Python. The following libraries were used:

*   `pandas`
*   `seaborn`
*   `numpy`
*   `matplotlib.pyplot`
*   `scikit-learn` (specifically `train_test_split`, `LinearRegression`, `mean_squared_error`, and `r2_score`)
*   `plotly.express`
*   `missingno`

## Dataset

The dataset used for this analysis is `vehicles.csv`. This dataset is included in the repository. It contains information on 426,880 used cars and has the following columns (among others):

*   `id`: Unique identifier for each listing
*   `region`: Geographic region of the listing
*   `price`: Price of the car
*   `year`: Year the car was manufactured
*   `manufacturer`: Car manufacturer
*   `model`: Car model
*   `condition`: Condition of the car
*   `cylinders`: Number of cylinders
*   `fuel`: Type of fuel
*   `odometer`: Mileage of the car
*   `title_status`: Status of the car's title
*   `transmission`: Type of transmission
*   `drive`: Drive type (e.g., 4WD, FWD)
*   `size`: Size of the car
*   `type`: Type of car (e.g., sedan, SUV)
*   `paint_color`: Color of the car
*   `state`: State where the car is located

## Data Analysis Process


The analysis followed these main steps:

1.  **Data Visualization:** The dataset was initially visualized to understand its structure and identify potential issues.
2.  **Data Cleaning:** Extreme values were removed to improve the quality of the data.
3.  **Data Preprocessing:** Further preprocessing steps were performed, which will be detailed in the code.
4.  **Data Splitting:** The data was split into training and testing sets.
5.  **Model Building:** Machine learning models were trained to predict car prices.

## Machine Learning Models

The following machine learning models were used:

*   **Linear Regression:** A baseline model assuming a linear relationship between features and price.
*   **Ridge Regression:** A regularized version of linear regression to prevent overfitting.
*   **XGBoost (Extreme Gradient Boosting):** A powerful gradient boosting algorithm capable of capturing complex non-linear relationships.

## Key Findings

The key finding is that XGBoost significantly outperformed both linear regression and ridge regression. This indicates a complex, non-linear relationship between car features and price.  While specific feature importance analysis was not performed in this initial phase, the superior performance of XGBoost suggests it effectively utilizes a combination of features and their interactions.

## Recommendations to the Used Car Dealership

1.  **Use XGBoost for Pricing:** Employ XGBoost (or similar gradient boosting algorithms) as the primary pricing model for used cars due to its superior accuracy.

2.  **Conduct Feature Importance Analysis:** Perform feature importance analysis to identify the most influential factors driving car prices. This will inform inventory management, marketing, and pricing strategies.

3.  **Collect More Data:** Consider gathering additional data like vehicle history, market data, and customer demographics to further refine the model.

4.  **Regularly Update the Model:** Continuously retrain and update the model with new data to reflect the dynamic used car market.

5.  **A/B Test Pricing Strategies:** Implement A/B testing to evaluate the effectiveness of different pricing strategies derived from the model.

6.  **Consider a Tiered Pricing Approach:** Develop a tiered pricing structure based on feature importance, offering premium prices for vehicles with the most desirable features.

7.  **Integrate with Inventory Management:** Integrate the pricing model with the inventory management system for automated price adjustments based on market conditions.


The analysis followed these main steps:

1.  **Data Visualization:** The dataset was initially visualized to understand its structure and identify potential issues.
2.  **Data Cleaning:** Extreme values were removed to improve the quality of the data.
3.  **Data Preprocessing:** Further preprocessing steps were performed, which will be detailed in the code.
4.  **Data Splitting:** The data was split into training and testing sets.
5.  **Model Building:** A machine learning model was trained to predict car prices.

## Machine Learning Model

A Linear Regression model was used to predict car prices.  Further details about the model and its evaluation will be provided in the code and analysis documentation.

What machine learning models were used?

Linear Regression: A basic model assuming a linear relationship between features and the target variable (car price).
Ridge Regression: A regularized version of linear regression, which helps prevent overfitting, especially when there are many features or some features are correlated.
XGBoost (Extreme Gradient Boosting): A powerful gradient boosting algorithm that builds an ensemble of decision trees. XGBoost is known for its ability to handle complex non-linear relationships and interactions between features.
Key Findings and Most Important Factors Influencing Car Prices:

The most important finding is that non-linear models, particularly XGBoost, significantly outperformed linear regression and ridge regression. This strongly suggests that the relationship between car features and price is complex and non-linear.  Simply put, car prices aren't just a straight line relationship with mileage or year.

While the analysis so far hasn't specifically identified which features are most important (feature importance analysis would be the next step), the improved performance of XGBoost indicates that it's effectively using a combination of features and their interactions to predict prices.  To get the most important features, you would want to use feature importance methods.

Specific Recommendations to the Used Car Dealership:

Use XGBoost (or a similar advanced model) for pricing:  Based on the superior performance, XGBoost (or other gradient boosting algorithms like LightGBM or CatBoost) should be the primary model used for pricing used cars.  This will lead to more accurate and competitive pricing.

Conduct Feature Importance Analysis:  Use feature importance analysis techniques (available in XGBoost and other tree-based models) to identify the most influential factors affecting car prices. This information is crucial for:

Inventory Management: Focus on acquiring and stocking vehicles with the most desirable features.
Marketing: Highlight the key selling points of cars based on what drives price.
Pricing Strategy: Develop more nuanced pricing strategies based on the relative importance of different features.
Collect More Data (If Possible):  Consider collecting additional data that might be relevant to car prices.  This could include:

Detailed vehicle history: Accident records, maintenance history, number of previous owners, etc.
Market data: Current market prices for similar models in the region.
Customer demographics: Understanding the preferences of different customer segments.
Regularly Update the Model:  The used car market is dynamic.  Regularly retrain and update your pricing model with new data to ensure it remains accurate and reflects current market conditions.

A/B Test Pricing Strategies:  Implement A/B testing to evaluate the effectiveness of different pricing strategies derived from the model.  This will help you fine-tune your pricing and maximize profitability.

Consider a Tiered Pricing Approach:  Based on the feature importance analysis, you might consider a tiered pricing approach.  For example, vehicles with the most desirable features could be priced at a premium, while those with less desirable features could be priced more competitively.

Integrate with Inventory Management:  Integrate the pricing model with your inventory management system.  This will allow you to automatically adjust prices based on market conditions and inventory levels.

By implementing these recommendations, the used car dealership can leverage machine learning to make more informed decisions about pricing, inventory, and marketing, ultimately leading to increased profitability and competitiveness.







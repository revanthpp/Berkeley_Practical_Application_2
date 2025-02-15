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
5.  **Model Building:** A machine learning model was trained to predict car prices.

## Machine Learning Model

A Linear Regression model was used to predict car prices.  Further details about the model and its evaluation will be provided in the code and analysis documentation.









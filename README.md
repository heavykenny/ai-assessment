# California Housing Price Prediction

## Overview
This project aims to predict median house values in Californian districts, based on various metrics such as median income, housing median age, and geographical location. It leverages a dataset from Kaggle, which includes features like the total number of rooms, bedrooms, population, and proximity to the ocean.

## Data Source
The dataset is sourced from Kaggle's "California Housing Prices" dataset, originally from the StatLib repository, which is based on the 1990 California census data. It can be found here: [California Housing Prices Dataset](https://www.kaggle.com/datasets/camnugent/california-housing-prices/data).

## Dependencies
- Python 3.x
- pandas
- matplotlib
- seaborn
- scikit-learn

## Installation
To install the required Python packages, run the following command:
```bash
pip install pandas matplotlib seaborn scikit-learn
```

## Data Preprocessing
- **Encoding Categorical Variables**: The `ocean_proximity` feature is one-hot encoded to convert categorical data into a numerical format.
- **Feature Scaling**: The features and target variable are standardized to have a mean of zero and a standard deviation of one. This is crucial for models that are sensitive to the scale of input features.

## Model Selection
Several regression models are evaluated:
- Linear Regression
- Lasso Regression
- Ridge Regression
- Decision Tree Regression
- Random Forest Regression

## Model Evaluation
Models are evaluated based on the Mean Squared Error (MSE) and R² score. Predictions are also scaled back to their original values for practical interpretability.

## Usage
1. **Data Loading**: Load the data using pandas' `read_csv` function.
2. **Initial Data Exploration**: Utilize descriptive statistics and visualizations to understand the dataset.
3. **Data Preprocessing**: Handle missing values, encode categorical variables, and scale features.
4. **Model Training and Evaluation**: Train the regression models and evaluate their performance.

## Future Work
- Experiment with more advanced regression models and tuning hyperparameters.
- Incorporate additional features that might improve the model's accuracy.
- Deploy the model as a web application for real-time predictions.

## Contributing
Contributions to improve the accuracy of the model or the efficiency of the code are welcome. Please ensure to follow the project's code style and add unit tests for any new features.


## Note
This is a school project for Artificial Intelligence Techniques (CSY3025)
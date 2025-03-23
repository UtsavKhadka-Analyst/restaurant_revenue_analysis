# Restaurant Revenue Analysis Using GAM and Lasso Regression

## Project Overview
This project analyzes restaurant revenue data to predict restaurant revenue based on various features such as rating, location, and menu characteristics. The analysis leverages two machine learning models: **Generalized Additive Models (GAM)** and **Lasso Regression** to capture complex relationships between features and predict the target variable, which is the restaurant's revenue.

## Table of Contents
1. [Project Overview](#project-overview)
2. [Data](#data)
3. [Analysis](#analysis)
   - [Generalized Additive Models (GAM)](#generalized-additive-models-gam)
   - [Lasso Regression](#lasso-regression)
4. [Visualizations](#visualizations)
5. [Requirements](#requirements)
6. [Usage](#usage)
7. [License](#license)

## Data
The dataset used in this analysis contains information about restaurant ratings, revenue, location, menu types, and more. The data is stored in an Excel file and contains multiple columns, including:
- `Rating`: The restaurant's average rating.
- `Revenue`: The revenue of the restaurant.
- `Location`: The location of the restaurant.
- `Menu_Type`: Type of menu offered (e.g., vegan, non-vegan).
- Other features related to the restaurant's characteristics.

## Analysis
The analysis involves using two different models to understand and predict the restaurant revenue:

### Generalized Additive Models (GAM)
GAMs were used to model non-linear relationships between the features and the target variable, i.e., revenue. The model was able to account for more complex relationships than traditional linear models.

**Key steps:**
1. Preprocessing of data (feature scaling, encoding categorical variables).
2. Building the GAM model and fitting it to the data.
3. Analyzing the partial dependence plots for feature importance.

### Lasso Regression
Lasso Regression was applied to identify the most important features influencing restaurant revenue and perform feature selection. Lasso regression helps shrink the less important feature coefficients to zero, ensuring a simpler and more interpretable model.

## Visualizations
Below are some of the key visualizations generated during the analysis:

- **Partial Dependence Plot for Rating**: Shows how the restaurant rating impacts the predicted revenue.
- **Correlation Matrix**: Visualizes the correlation between different features in the dataset.
- **Model Performance**: Plots the performance metrics (e.g., R-squared, Mean Squared Error) of the models.

## Requirements
To run the analysis locally, ensure that you have the following Python libraries installed:

- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `sklearn`
- `pygam` (for GAM)
- `statsmodels`
- `openpyxl` (for reading Excel files)

Install the required libraries using:

```bash
pip install pandas numpy matplotlib seaborn sklearn pygam statsmodels openpyxl

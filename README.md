# Restaurant Revenue Analysis

This project focuses on analyzing restaurant revenue data to identify key factors influencing revenue and to predict future revenue based on features such as restaurant ratings, cuisine type, and other factors. The analysis leverages **Generalized Additive Models (GAM)** for capturing non-linear relationships and **Lasso Regression** for feature selection and predictive modeling.

## Table of Contents
1. [Project Description](#project-description)
2. [Installation](#installation)
3. [Usage](#usage)
4. [Data](#data)
5. [Analysis](#analysis)
6. [Results](#results)
7. [Contributing](#contributing)
8. [License](#license)

## Project Description

The objective of this analysis is to explore the relationship between various restaurant features and their revenue. The project performs a deep dive into the data, visualizing trends and building predictive models using **Lasso Regression** and **Generalized Additive Models (GAM)**. The insights from these models aim to help restaurant managers and analysts understand the factors influencing revenue.

## Installation

Clone the repository to your local machine or access it via Google Colab for easy execution.

### Clone the Repository

To clone the repository, run the following command:

```bash
git clone https://github.com/UtsavKhadka-Analyst/restaurant-revenue-analysis.git


Usage

To run the analysis, follow these steps:

Clone this repository to your local machine or open it in Google Colab:

git clone https://github.com/YourGitHubUsername/restaurant-revenue-analysis.git

Open the Jupyter Notebook or Google Colab notebook (Utsav_Khadka_FE.ipynb) to view the code and analysis.
Ensure you have the necessary dataset (restaurant_revenue_MT.xlsx) available in your working directory.
Run the cells in the notebook for data preprocessing, feature engineering, and model training.

Data

The dataset restaurant_revenue_MT.xlsx includes the following columns:

Rating                   0
Seating Capacity         0
Average Meal Price       0
Ambience Score           0
Service Quality Score    0
Weekend Reservations     0
Weekday Reservations     0
Revenue_Cat

Analysis Details

1. Lasso Regression
Lasso regression is used to regularize the linear regression model and helps with feature selection. It penalizes the coefficients of less important features, effectively shrinking them to zero.

from sklearn.linear_model import Lasso
lasso = Lasso(alpha=0.1)
lasso.fit(X_train, y_train)
This part of the analysis focuses on how restaurant features affect revenue by selecting the most influential features using Lasso.

2. Generalized Additive Models (GAM)
GAM is used to model the non-linear relationships between the features and the target variable (revenue). In this analysis, we apply GAM to understand how features like Rating and Review Count non-linearly influence revenue.

from pygam import LinearGAM, s
gam = LinearGAM(s(0) + s(1)).fit(X_train, y_train)
This model allows us to visualize and interpret the influence of the individual features on restaurant revenue.




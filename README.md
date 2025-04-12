# Seoul-Bike


This project is a collaboration with:

- [@shahdayman11](https://github.com/shahdayman11) 
- [@malakelsayed2](https://github.com/malakelsayed2)

Thanks to both for their valuable contributions!

In this project, We developed predictive models to estimate the number of rented bikes (Rented Bike Count) using multiple machine learning techniques and feature transformations. We explored both simple and multiple regression models, incorporating polynomial features to capture non-linear relationships. The steps involved include:

Data Preprocessing:

The dataset was split into training and testing sets (90% train, 10% test).

Features like Temperature(°C), Humidity(%), Solar Radiation (MJ/m2), and others were selected based on their influence on bike rentals.

Model Development:

Simple Linear Regression: Initially, a simple linear regression model was built using only Temperature(°C) to predict Rented Bike Count.

Multiple Linear Regression: A multiple linear regression model was then created with a broader set of features, including Dew point temperature(°C), Hour, Humidity(%), and others.

Polynomial Ridge Regression: Polynomial features (degree 2, 3, and 4) were applied to capture non-linear relationships, followed by Ridge Regression (L2 regularization) to prevent overfitting.

Evaluation:

The models were evaluated using Mean Squared Error (MSE) and R² Score, which measured the accuracy and fit of the models.

R² values were reported to assess how well the models explained the variance in the target variable.

Findings:

Ridge Regression with polynomial features improved the model’s ability to capture more complex patterns in the data.

Models with higher polynomial degrees (e.g., degree 4) and additional features showed better prediction accuracy, although regularization (alpha=1) was essential for controlling overfitting.

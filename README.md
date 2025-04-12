# Seoul-Bike


This project is a collaboration with:

- [@shahdayman11](https://github.com/shahdayman11) 
- [@malakelsayed2](https://github.com/malakelsayed2)

Thanks to both for their valuable contributions!

In this project, We conducted a comprehensive analysis using the Seoul Bike Sharing Dataset from Kaggle to build models that predict the number of bikes rented based on environmental and time-related features. The workflow was split into regression and classification tasks, with the following methodology:

Data Preprocessing:

The dataset was split into training and testing sets (90% train, 10% test).

Features like Temperature(°C), Humidity(%), Solar Radiation (MJ/m2), and others were selected based on their influence on bike rentals.

Regression Models: Predicting Rented Bike Count
1. Simple Linear Regression
Feature used: Temperature(°C)

The dataset was split (80/20), scaled using StandardScaler, and used to train a linear regression model.

The relationship between temperature and bike rentals was visualized, and model performance was evaluated using R² and MSE.

2. Multiple Linear Regression
Features used: Top contributors such as Temperature, Humidity, Hour, Dew Point, etc.

After scaling, the model was trained and evaluated. A scatter plot comparing actual vs. predicted values was generated.

3. Polynomial Ridge Regression
Explored non-linear relationships by applying polynomial features of degrees 2, 3, and 4.

Used Ridge Regression (L2 regularization) to prevent overfitting.

Applied to both:

Simple case with only Temperature

Multiple features selected based on feature importance

Model performance was evaluated using R² and MSE, showing improved accuracy with polynomial features and regularization.

Classification Task: Multi-Output Logistic Regression
4. MultiOutput Logistic Regression
A classification model was developed using LogisticRegression wrapped in MultiOutputClassifier to predict multiple binary targets simultaneously.

Features were scaled with StandardScaler to ensure equal importance.

The logistic regression model was trained on the training set with max_iter=200 to ensure convergence.

Conclusion:
Linear and Ridge regression models were effective in modeling bike rental counts, especially when using multiple features and polynomial degrees.

Ridge regularization controlled overfitting and maintained generalization.

The multi-output logistic regression model allowed for simultaneous prediction of multiple binary outcomes, offering insight into feature contributions for each classification task.

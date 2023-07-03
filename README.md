# Random-Forest-Regression-Model
A model that tests dataset based upon the working of Random Forest Regression

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Importing the necessary libraries:

numpy (as np): A library for numerical operations in Python.
matplotlib.pyplot (as plt): A library for creating visualizations in Python.
pandas (as pd): A library for data manipulation and analysis in Python.

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Importing the dataset:

The code assumes that there is a file named 'Position_Salaries.csv' in the same directory as the script.
The data is read using the read_csv function from pandas, and the independent variable (X) and dependent variable (y) are extracted from the dataset.

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Training the Random Forest Regression model:

The RandomForestRegressor class from scikit-learn is used to create a regression object named regressor.
The number of decision trees (n_estimators) is set to 10, and the random state is set to 0.
The fit method is called to train the model using the features (X) and target variable (y).

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Predicting the salary for a new data point:

The predict method of the regressor object is used to predict the salary for a new data point [[6.5]].
The predicted salary is printed.

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Visualizing the Random Forest Regression results:

A range of feature values (X_grid) is created using np.arange to create a smooth curve for visualization.
The feature values are reshaped using reshape to be compatible with the predict method.
A scatter plot is created using the original feature values (X) and salaries (y) to visualize the actual data points.
The Random Forest Regression predictions for the feature values in X_grid are plotted as a blue line on the scatter plot.

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
The plot is given a title and labels for the x-axis and y-axis using plt.title, plt.xlabel, and plt.ylabel.
The plot is shown using plt.show().
The code performs Random Forest Regression on the provided dataset, trains the model, predicts the salary for a new data point, and visualizes the actual data points and the Random Forest Regression predictions.

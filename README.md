# Car Price Prediction

This Python code performs a predictive analysis on a dataset related to car sales. The main steps in the code are as follows:

1. **Importing Libraries:**
   - `numpy` for numerical operations
   - `pandas` for data manipulation and analysis
   - `seaborn` and `matplotlib.pyplot` for data visualization
   - `train_test_split` from `sklearn.model_selection` for splitting the dataset into training and testing sets
   - `LinearRegression` and `Lasso` from `sklearn.linear_model` for building linear regression and Lasso regression models
   - `metrics` from `sklearn` for evaluating the model performance

2. **Loading the Dataset:**
   - Reads a CSV file ('car data.csv') into a pandas DataFrame (`car_dataset`).

3. **Data Exploration:**
   - Displays the first few rows of the dataset using `head()`.
   - Prints the shape of the dataset.
   - Checks for missing values in the dataset using `isnull().sum()`.
   - Counts the occurrences of different values in the 'Fuel_Type' column.

4. **Data Preprocessing:**
   - Converts categorical variables ('Fuel_Type', 'Seller_Type', 'Transmission') into numerical values.

5. **Splitting the Dataset:**
   - Divides the dataset into features (`X`) and the target variable (`Y`).
   - Splits the data into training and testing sets using `train_test_split`.

6. **Model Training:**
   - Initializes linear regression (`linear`) and Lasso regression (`lasso`) models.
   - Fits these models to the training data.

7. **Model Evaluation on Training Data:**
   - Predicts the selling prices on the training data using both linear and Lasso regression models.
   - Calculates R-squared scores for both models.

8. **Data Visualization:**
   - Creates scatter plots to visualize the relationship between actual and predicted selling prices for both linear and Lasso regression models on the training data.

9. **Model Evaluation on Testing Data:**
   - Predicts the selling prices on the test data using both linear and Lasso regression models.
   - Calculates R-squared scores for both models.

10. **Data Visualization on Testing Data:**
    - Creates scatter plots to visualize the relationship between actual and predicted selling prices for both linear and Lasso regression models on the test data.

In summary, the code aims to train linear and Lasso regression models on a car sales dataset, evaluate their performance on both training and testing sets, and visualize the predicted prices against the actual prices. The R-squared scores and scatter plots provide insights into how well the models capture the variability in the selling prices.

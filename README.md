# CodeAlpha - Car Price Prediction with Machine Learning
## Project Overview
This project is part of my **CodeAlpha Data Science Internship**.
The objective of this project is to predict the selling price of used cars using machine learning. A **Linear Regression** model was developed using car-related features such as present price, car age, kilometers driven, fuel type, transmission, and ownership.
The project includes data cleaning, feature engineering, categorical data preprocessing, model training, prediction, evaluation, and visualization.

## Objectives
- Analyze the car price dataset
- Perform data cleaning and preprocessing
- Handle duplicate records
- Create a new Car Age feature
- Convert categorical variables into numerical variables
- Build a Linear Regression model
- Predict car selling prices
- Evaluate model performance
- Visualize the relationship between actual and predicted prices

## Dataset
The dataset initially contains **301 car records**.
The dataset includes car-related information such as:
- Year
- Present_Price
- Selling_Price
- Kms_Driven
- Fuel_Type
- Seller_Type
- Transmission
- Owner
The target variable is:
**Selling_Price**

## Technologies Used
- Python
- Jupyter Notebook
- Pandas
- Matplotlib
- Scikit-learn

## Project Workflow
### 1. Import Libraries
The following Python libraries were used:
- Pandas
- Matplotlib
- Scikit-learn

### 2. Load the Dataset
The car dataset was loaded using Pandas.

### 3. Data Exploration
The dataset was explored using:
- `head()`
- `shape`
- `columns`
- `info()`
- `describe()`

### 4. Data Quality Checking
The dataset was checked for:
- Missing values
- Duplicate records
Two duplicate records were removed during data cleaning.

### 5. Feature Engineering
A new feature called **Car_Age** was created using the Year column.
The calculation used was:
Car_Age = 2026 - Year

### 6. Feature and Target Selection
The target variable was:
**Selling_Price**
The remaining columns were used as input features.

### 7. Categorical Data Preprocessing
Categorical variables were converted into numerical variables using **One-Hot Encoding** with `pd.get_dummies()`.

### 8. Train-Test Split
The dataset was divided into:
- 80% Training Data
- 20% Testing Data
A random state of 42 was used.

### 9. Model Building
A **Linear Regression** model was created using Scikit-learn.
The model was trained using the training dataset.

### 10. Prediction
The trained model was used to predict car selling prices for the test dataset.

### 11. Model Evaluation
The model was evaluated using:
- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- R² Score
The model achieved an **R² score of approximately 0.75**.

## Data Visualizations
The project includes the following visualizations:
### 1. Actual vs Predicted Car Prices
A scatter plot was created to compare the actual selling prices with the prices predicted by the Linear Regression model.

### 2. Present Price vs Selling Price
A scatter plot was created to understand the relationship between the present price of a car and its selling price.
The visualization shows a strong relationship between Present Price and Selling Price.

### 3. Distribution of Car Selling Prices
A histogram was created to show the distribution of car selling prices in the dataset.

## Key Findings
- The dataset initially contained **301 car records**.
- Two duplicate records were removed during data cleaning.
- A new **Car_Age** feature was created using the Year column.
- Categorical variables were converted into numerical variables using One-Hot Encoding.
- Linear Regression was used to predict car selling prices.
- The model achieved an **R² score of approximately 0.75**.
- Present Price shows a strong relationship with Selling Price.
- Car-related features can be used to support data-driven price prediction.

## Real-World Application
Car price prediction can help:
- Used-car dealers estimate suitable selling prices.
- Customers understand the expected value of a used car.
- Businesses make data-driven pricing decisions.
- Dealers analyze factors that influence car prices.
Machine learning can use factors such as present price, car age, kilometers driven, fuel type, transmission, and ownership to support car price prediction.

## Conclusion
In this project, a **Linear Regression model** was developed to predict car selling prices.
The project included data exploration, data cleaning, feature engineering, categorical data preprocessing, train-test splitting, model training, prediction, model evaluation, and data visualization.
The model achieved an **R² score of approximately 0.75**, demonstrating that machine learning can be applied to predict used-car selling prices based on available car features.

## Files in this Repository
- `CodeAlpha_Car_Price_Prediction.ipynb` - Jupyter Notebook containing the complete analysis, machine learning model, outputs, and visualizations
- `car.csv` - Dataset used for car price prediction
- `README.md` - Project documentation

## Internship
This project was completed as part of my **CodeAlpha Data Science Internship**.

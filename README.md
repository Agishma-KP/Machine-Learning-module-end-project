# Car Price Prediction Project

## Project Overview
This project aims to analyze and predict car prices in the American market. A Chinese automobile company plans to enter the US market and needs insights into the key factors affecting car pricing. Using machine learning regression models, we determine which variables significantly impact car prices and how well they predict the price.

## Dataset
**Filename:** `CarPrice_Assignment.csv`  
**Source:** Provided by the consulting firm after market surveys  
**Description:** The dataset contains information on various car attributes, such as make, model, engine type, horsepower, fuel type, and more.

### Features in the Dataset:
- `Car_ID`: Unique identifier for each car
- `CarName`: Name of the car model
- `Fueltype`: Type of fuel used (e.g., gas, diesel)
- `Aspiration`: Type of aspiration system (e.g., turbo, standard)
- `Horsepower`: Engine power output
- `Wheelbase`: Distance between the front and rear axles
- `Curbweight`: Weight of the vehicle
- `Highwaympg`: Mileage on highways
- `Price`: The target variable (car price in USD)
- ... and more

## Methodology
### **1. Data Preprocessing**
- Load the dataset
- Handle missing values and duplicates
- Encode categorical variables (e.g., `LabelEncoder` for fuel type, aspiration)
- Scale numerical features using `StandardScaler`
- Transform skewed features using `PowerTransformer`
- Select important features using `SelectKBest`

### **2. Model Implementation**
Five regression models were trained and evaluated:
1. **Linear Regression**
2. **Decision Tree Regressor**
3. **Random Forest Regressor**
4. **Gradient Boosting Regressor**
5. **Support Vector Regressor (SVR)**

### **3. Model Evaluation**
Each model was assessed using:
- **R-squared (R²)**: Measures how well the model fits the data
- **Mean Squared Error (MSE)**: Measures the average squared error
- **Mean Absolute Error (MAE)**: Measures the average absolute error

### **4. Feature Importance Analysis**
- Used feature importance from `RandomForestRegressor` and `GradientBoostingRegressor` to identify key variables affecting car prices.

### **5. Hyperparameter Tuning**
- `GridSearchCV` was used to optimize the models and improve performance.

## Results
- The best-performing model was selected based on R², MSE, and MAE.
- Feature importance analysis showed that attributes like `horsepower`, `curbweight`, and `engine size` had the most influence on price.

## How to Run the Project
1. Install the required dependencies:
   ```sh
   pip install pandas numpy matplotlib seaborn scikit-learn
   ```
2. Open the Jupyter Notebook and run all cells.
3. The dataset should be placed in the same directory as the notebook.
4. The final results, including model evaluations and visualizations, will be displayed.

## Submission
- The project is submitted as a Jupyter Notebook (.ipynb) on GitHub.
- Ensure all explanations, code, and outputs are clear.

## Contact
For any queries, feel free to reach out via GitHub issues or email.

---
**Author:** Agishma K P 
**Date:** 29 March 2025


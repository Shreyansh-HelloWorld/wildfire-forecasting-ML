# wildfire-forecasting-ML

# Fire Weather Prediction using Machine Learning

This repository contains a machine learning project focused on predicting **Fire Weather Index (FWI)** using meteorological data. The project applies feature engineering, data preprocessing, and multiple regression techniques, including **Linear Regression, Lasso, Ridge, and ElasticNet**.

## Project Overview

### **Dataset**
- The dataset used in this project is **Algerian_ff_cleaned_dataset.csv**.
- The target variable is **FWI (Fire Weather Index)**.
- The dataset includes various meteorological attributes, with categorical values encoded into numerical format.

### **Machine Learning Pipeline**
1. **Data Preprocessing**
   - Dropped unnecessary columns (`day`, `month`, `year`).
   - Converted categorical class labels (`Classes`) into binary values (0 for "not fire" and 1 for "fire").
   - Identified and removed highly correlated features (correlation threshold = 0.85).
   - Applied feature scaling using **StandardScaler**.

2. **Model Training & Evaluation**
   - **Linear Regression**: Used to establish baseline performance.
   - **Lasso Regression**: Applied to reduce feature complexity.
   - **Ridge Regression**: Added L2 regularization to prevent overfitting.
   - **ElasticNet Regression**: A combination of Lasso and Ridge.
   - **Evaluation Metrics**: 
     - **Mean Absolute Error (MAE)**
     - **R² Score**
   - Visualized model performance using scatter plots.

## Installation

Make sure you have Python 3 installed. Install the required dependencies using:

`pip install pandas numpy matplotlib seaborn scikit-learn`

How to Run
Clone the repository:


`git clone https://github.com/<your-username>/fire-weather-prediction.git`
`cd fire-weather-prediction`

Ensure the dataset Algerian_ff_cleaned_dataset.csv is present in the project directory.

Run the Jupyter Notebook:

`jupyter notebook Model_Training.ipynb`

Results
The Linear Regression model provides baseline predictions with an R² score indicating model fit.
Lasso & Ridge regressions improve generalization by preventing overfitting.
ElasticNet balances between feature selection and regularization.
Contributing
If you want to contribute, feel free to fork the repository and submit a pull request with improvements.

License
This project is licensed under the MIT License.

Acknowledgements
This project was inspired by fire risk prediction datasets and meteorological forecasting techniques.

---

This README clearly explains the project scope, models used, dataset, and setup instruct

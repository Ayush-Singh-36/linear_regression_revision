# Medical Insurance Cost Prediction using Linear Regression

## Project Overview

This project aims to predict medical insurance costs using linear regression. The analysis is performed on the `insurance.csv` dataset, which contains demographic and health information for individuals.

## Dataset

The dataset used is `insurance.csv`, containing the following columns:
- `age`: age of primary beneficiary
- `sex`: insurance contractor gender, female, male
- `bmi`: Body mass index, providing an understanding of body, weights that are relatively high or low relative to height, objective index of body weight (kg / m^2) using the ratio of height to weight, ideally 18.5 to 24.9
- `children`: number of children covered by health insurance / number of dependents
- `smoker`: smoking status
- `region`: residential area of the beneficiary in the US (northeast, southeast, southwest, northwest)
- `charges`: individual medical costs billed by health insurance

## Analysis Steps

The notebook covers the following key steps:
1.  **Data Loading and Initial Exploration**: Loading the dataset using pandas and performing initial data overview.
2.  **Exploratory Data Analysis (EDA)**: Visualizing distributions of key features like age, BMI, and charges. Analyzing the relationship between charges and other variables, particularly smoking status.
3.  **Feature Engineering**: 
    - Converting categorical features (`smoker`, `sex`, `region`) into numerical representations using mapping and one-hot encoding.
    - Scaling numerical features (`age`, `bmi`, `children`) using `StandardScaler`.
4.  **Model Building (Linear Regression)**:
    - Implementing a simple linear regression model from scratch to understand the basic concept.
    - Using `sklearn.linear_model.LinearRegression` to build models for predicting charges, first with a single feature (age) and then with multiple features.
    - Evaluating model performance using Root Mean Squared Error (RMSE).

## Technologies Used

-   Python
-   Pandas (for data manipulation)
-   NumPy (for numerical operations)
-   Matplotlib & Plotly Express (for data visualization)
-   Scikit-learn (for linear regression models and preprocessing)

## How to Run the Notebook

1.  **Clone the repository**: (Assuming this notebook will be in a GitHub repo)
    ```bash
    git clone <repository-url>
    cd <repository-name>
    ```
2.  **Ensure you have the dataset**: Make sure `insurance.csv` is in the same directory as the notebook.
3.  **Install dependencies**: Install the required Python libraries:
    ```bash
    pip install pandas numpy matplotlib seaborn plotly scikit-learn
    ```
4.  **Open the notebook**: Open the `.ipynb` file in a Jupyter environment (e.g., Jupyter Lab, Google Colab).
5.  **Run cells sequentially**: Execute the cells in the notebook from top to bottom.

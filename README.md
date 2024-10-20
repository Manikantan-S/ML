# ML Project House Price Prediction

## Overview
This repository contains an implementation of Ridge Regression, alongside the evaluation of its performance and comparison with other machine learning algorithms like Gradient Boosting Regressor, Support Vector Regressor, Random Forest, K-Neighbors Regressor, and AdaBoost Regressor. The goal is to predict target values from given features while minimizing error, with performance measured using RMSE (Root Mean Squared Error) and R² scores.

## Code Structure
The code is organized into several cells for clarity and ease of execution. Below is a brief explanation of each section:

### 1. Import Libraries
In the first cell, necessary libraries such as NumPy and `mean_squared_error` from sklearn are imported to facilitate calculations.

### 2. Manual Ridge Regression Function
This function implements the manual computation of Ridge Regression. It adds a bias term to the feature matrix and calculates the weights (theta) using the closed-form solution of Ridge Regression:

**θ = (Xᵀ * X + α * I)⁻¹ * Xᵀ * y**

Where:
- **X** is the input matrix
- **y** is the output vector
- **α** is the regularization parameter
- **I** is the identity matrix
### 3. Predictions Function
This function generates predictions for multiple alpha values by invoking the manual Ridge Regression function and storing the results in a dictionary.

### 4. Specify Alpha Values
A range of alpha values is defined, which are used to assess the impact of regularization strength on model performance.

### 5. Get Ridge Predictions
The predictions for each alpha value are obtained by calling the predictions function.

### 6. Calculate and Print Scores
For each set of predictions, the R² score and RMSE are calculated and printed. The R² score indicates the proportion of variance explained by the model, while RMSE provides a measure of the average error in the predictions.

## Results
Below are the RMSE errors and corresponding accuracy for each alpha used in the Ridge Regression model:

| Alpha     | RMSE   | R^2          |
|-----------|--------|--------------|
| 0.01      | 0.0002 | 1.0        |
| 0.1       | 0.0010 | 1.0       |
| 1.0       | 0.0092 | 0.9995        |
| 10.0      | 0.0562 | 0.9795      |
| 100.0     | 0.1172 | 0.9111       |

**Final Ridge Regression Metrics**:
- **R² is**: 0.9111059
- **RMSE is**: 3.62393044021158e-05 (indicating an accuracy of approximately 99%).

### Other Methods Used
The following algorithms were also implemented and their respective performances measured:

| Methods                     | RMSE       |
|-------------------------------|------------|
| Support Vector Regressor (SVR) | 0.20379    |
| Random Forest                  | 0.01066    | 
| K-Neighbors Regressor          | 0.21668    |
| AdaBoost Regressor             | 0.02386    | 
## Outputs 
![{C2AAE3DE-DF4D-4325-9457-D2DE5FFE2BCA}](https://github.com/user-attachments/assets/733f10d7-2f9f-4b28-b05e-57b3696ae51a)
![image](https://github.com/user-attachments/assets/3ee16e4c-d496-4601-99af-88b5feed7929)
![image](https://github.com/user-attachments/assets/e87669fa-948f-4f39-af53-8298e8d7643c)
![image](https://github.com/user-attachments/assets/573feb99-27dd-4bc9-a7aa-2a3538b60864)
![image](https://github.com/user-attachments/assets/b84135a4-dafd-4469-a93e-854e309390dd)
![image](https://github.com/user-attachments/assets/e1c21693-56ae-4867-a18a-077780729c5e)

## Contribution
This project was made by the following contributors:

| Registration Number | Name                      |
|---------------------|---------------------------|
| RA2211003010398     | Rishav Prakash            |
| RA2211003010436     | P Karthik Manikantan      |
| RA2211003010446     | Ujan Pradhan              |
| RA2211003010464     | Krishna Chitanya          |



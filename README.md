# Simple Local Regression for Mortality Rate Prediction

This project explores the use of **local linear regression** to predict mortality rates (`MORT`) based on the percentage of families living in poverty (`POOR`). The dataset can be found in the file "pollution_cleaneddata.csv" with the code in the notebook file "Exercise_LinearRegression.ipynb". 

The regression is formulated as a weighted least-squares optimization problem, where nearby observations are given different weights according to their distance from the prediction point.

The project compares **three weighting methods** and investigates how the choice of the number of neighboring observations affects the fitted regression and prediction accuracy. The models are used to estimate mortality rates for poverty levels of **10%, 18%, and 25%**, including the corresponding standard errors.

The repository contains the implementation, visualizations, and results used to evaluate the different weighting strategies and neighborhood sizes.

# Insurance-Cost-Prediction-Regression
Predict the insurance cost (charges) for individuals based on demographic and health-related features.

## <b>PROBLEM CONTEXT
<b>

-  Affordable health insurance to thousands of customer. You're tasked with creating an automated system to estimate the annual medical expenditure for new customers, using information such as their age, sex, BMI, children, smoking habits and region of residence.
-  Estimates from your system will be used to determine the annual insurance premium (amount paid every month) offered to the customer.


### <b>TYPE OF MACHINE LEARNING PROBLEM.
- <b>It is a Regression problem, where given the above set of features, we need to estimate the annual medical expenditure for new customers.<br>
### <b>LIST OF ALGORITHMS USES FOR Regression
<b>
    
- Linear Regression
- KNeighborsRegressor
- DecisionTreeRegressor
- RandomForestRegressor
- GradientBoostingRegressor
- XGBRegressor


## <b>DATASET OVERVIEW

#### <b>Feature	Description
- <b>Age</b><br>Age of the person
- <b>Sex</b><br>Gender (male/female)
- <b>BMI</b><br>Body Mass Index
- <b>Children</b><br>Number of dependent children
- <b>Smoker</b><br>Smoking status (yes/no)
- <b>Region</b><br>Residential area
- <b>Charges</b><br>Annual insurance charges (Target)


# <b>TASK 1
### <b>PREPARE A COMPLETE DATA ANALYSIS REPORT ON THE GIVEN DATA.

# <b>TASK 2
### <b>Prepare the data, identifying and extracting key features (both input and output parameters) relevant to the problem you will solve.
### <b>Build and train a machine learning model. Here you can evaluate different algorithms, settings and see which model is best for your scenario


## <b>Model Performance Comparison (Before vs After Hyperparameter Tuning)
| **Model**                     | **RMSE Before** | **RMSE After** | **R² Before** | **R² After** | **Comments**                                             |
| ----------------------------- | --------------- | -------------- | ------------- | ------------ | -------------------------------------------------------- |
| **Linear Regression**         | 5956.34         | 5821.63        | 0.81          | 0.77         | Slight RMSE improvement, minor drop in R²                |
| **KNeighborsRegressor**       | 5819.21         | 9872.54        | 0.76          | 0.32         | RMSE and R² worsened—model underperforms after tuning    |
| **RandomForestRegressor**     | 4605.38         | 4621.09        | 0.85          | 0.85         | Performance stable, hyperparameters had minimal effect   |
| **GradientBoostingRegressor** | 5819.21         | 4482.26        | 0.86          | 0.86         | RMSE improved significantly with tuning, R² unchanged    |
| **XGBRegressor**              | 5819.21         | 4483.77        | 0.82          | 0.86         | Large performance boost from tuning; best generalization |
| **DecisionTreeRegressor**     | 5819.21         | 4770.01        | 0.84          | 0.84         | RMSE dropped with tuning, R² stayed constant             |

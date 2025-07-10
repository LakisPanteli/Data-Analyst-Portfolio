# Bike Rental Analysis
## Introduction
<p>In this project I will be trying to find the Machine Learning method that best predicts the count of total rental bikes (‘cnt’) each day over a two-year period. That means I will be measuring the test error rates of each method and the one with the least test error will be the one that most accurately predicts ‘cnt’. I shall use the test mean squared error (MSE) to measure how close the predicted response value for a given observation is to the true response value for that observation. The smaller the value of the test MSE, the closer the predicted responses are to the true response value.</p>
<p>The methods I will be using are multiple linear regression, best subset selection, forward and backward stepwise selection, Ridge regression, the Lasso, Principal Components Regression (PCR), Partial Least Squares (PLS), Generalised Additive Models (GAM), Regression Trees, Bagging, Random Forests and Boosting.</p>

## <p> Data and exploratory analysis </p>
<p>The data source I will be using to test these Machine Learning methods is the Bike Sharing Dataset, using the prediction of bike rental count daily (‘cnt’) based on environmental and seasonal settings. There are 731 observations and 16 variables. When analysing this data and applying the machine learning methods I shall not be using the variables ‘instant’, ‘dteday’, ‘registered’ and ‘casual’. This is because they add no value when analysing the data on ‘cnt’ because ‘instant’ is simply just the number of the observation and ‘registered’ and ‘casual’ add up to the value of ‘cnt’ so there is no need to keep them in. The variable ‘dteday’ will not be used because there are variables such as ‘yr’, ‘mnth’, ‘season’, ‘weekday’, ‘workingday’ and ‘holiday’ which cover for the specific day and in fact make the model easier to interpret as they are giving you a more general value of date and time. The variable ‘cnt’ is most correlated with ‘temp’, ‘atemp’, ‘season’, ‘yr’ and ‘weathersit’. I then created some boxplots, scatterplots and histograms to analyse what the data is showing.</p>

**<p> Box Plots**</p> 
<img width="554" height="291" alt="image" src="https://github.com/user-attachments/assets/6172d55e-cfa9-40e2-9a15-f5816e54e6e9" />
<img width="599" height="273" alt="image" src="https://github.com/user-attachments/assets/9d25771a-367e-4788-bf61-ae4809bfcff8" />
<img width="636" height="307" alt="image" src="https://github.com/user-attachments/assets/b3ce4f3c-ae57-48d8-a80d-a0947caa7f06" />
<img width="653" height="314" alt="image" src="https://github.com/user-attachments/assets/a897743d-d27d-489a-91d3-e8b38364fddf" />
<img width="628" height="304" alt="image" src="https://github.com/user-attachments/assets/79db87b5-52a6-4b77-952b-dc2a0c707c16" />

**<p> Scatterplots** </p>
<img width="575" height="486" alt="image" src="https://github.com/user-attachments/assets/2dd8a25f-3590-4450-bca3-45be68f54f38" />
<img width="601" height="447" alt="image" src="https://github.com/user-attachments/assets/7f74330f-8185-4c15-b6d7-f3dde387d2dc" />
<img width="522" height="435" alt="image" src="https://github.com/user-attachments/assets/b3d0801e-bc70-439e-a84a-321ebe026807" />
<img width="530" height="443" alt="image" src="https://github.com/user-attachments/assets/99603fb5-a448-48d0-9d49-9d7e275e2b67" />

**<p> Histogram** </p>
<img width="584" height="329" alt="image" src="https://github.com/user-attachments/assets/44e1660b-53bb-4ecf-8fa4-60835e548c03" />

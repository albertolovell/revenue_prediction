### User Interaction<br><br>
### Objective

This notebook is an exploration of anonymized data from a Bay Area Fin-Tech startup, and was collected from users interacting with the company website. The goal here is to explore trends given user_id, conversion status, channel through which the site was accessed, timestamp, and revenue contributed by each user. An ideal model will accurately predict any future user's revenue contribution based on their interaction with the platform. "Conversion" in this case represents any user who contributed to direct revenue gain.<br>



Since data is skewed, Mean Absolute Error will be the evaluation metric. Selecting a model which predicts all output revenue values to be the mean, the mean absolute error is approximately $156. This will be the baseline scoring metric. 

### Results

Comparing a Linear Regression, a KNN Regressor, and a RandomForest Regressor the RandomForest Regressor had the lowest MAE at $31.01. This is about 5x better than our baseline scoring metric and will give us the best possible prediction give the data.

### Data <br>
touches.csv : Details user interactions, across marketing channels<br>funnel.csv : Details user conversion status and revenue



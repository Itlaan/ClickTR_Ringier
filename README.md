# ClickTR_Ringier
 RingierAssignment for click through rate
 
 ## Assignment to develop a model for predicting click through rate based on given training data
Jupyter notebook included for:
    1. Exploratory data analysis (CTR_EDA_v00.pynb)
    2. Model development and prediction (CTR_PredModel_v01.pynb)

### Train Test Split 
Data split into 70/30% Train Test split

### Features and findings
unix_timestamp: Converted to datetime and weekdays and hours used. Higher click rate on weekends
f7: Only variable with Nulls/nans. Nulls showed > 40% click rate so nans were retained for modelling.
All other categorical fields were recoded so that only categories with significantly higher volumes were retained.
This reduced the dimensionality of the variables used in the model speeding up training time. 
Categories with low volume were dumped into 'Other' category.

### Feature selection
Used sklearn feature importance, specifically for RandomForest Classifier.
Used the the variables with highest importance contribution such that >= 80% of contribution was maintained.

Did not have time for model selection however would have been good to explore other models. 
Imbalanced dataset therefore F1 score and Poor Precision-Recall curve used.
Poor performance of model as < 40% F1 score. Poor Precision-Recall curve. 
Business problem assumption is that False Positive would be most important to minimise.
More EDA needed over all variables to improve performance as unlikely for another algorithm to surpass 50% F1 Score.

 

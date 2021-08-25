# [30 Days of ML](https://www.kaggle.com/c/30-days-of-ml)

![image](https://user-images.githubusercontent.com/34986276/130677626-5ac832fb-ba23-4f43-b621-ce999df4e3e4.png)

30 Days of ML on Kaggle was an in class prediction competition on a regression task.

First, I used the Random Forest Regression algorithm. 
I was very much constraint in performance using only CPU for processing (algorithm does not use GPU).
So I had to limit the dataset in order to complete training runs. This adversely affected results. 

[See RandomForest code here](https://github.com/andriescoetsee/my_first_kaggle_competition/blob/4921edfc802a2aa1c968ae869392150fbf53ad9f/30-days-of-ml-random-forest.ipynb)

Then, I used the XGBoost algorithm using the same framework, however this time utilization the full data set of 300,000 observations for training.
This algorithm utilizes GPU, what a pleasure it was to train the model, adjust parameters, retrain and then seeing how the RMSE (root mean squared error as loss metric) descreases. 

[See XGBoost code here](https://github.com/andriescoetsee/my_first_kaggle_competition/blob/f7237fce1afbd4183cc4e49d1a595238cee49315/30-days-of-ml-xgboost.ipynb)

## Conclusion

At the time of submission the #1 position produced a RMSE of 0.71727 while my own score came in at #1045 with RMSE 0.71948. 
In total there were close to 6,000 participants. The leaderboard was calculated with approximately 25% of the test data. While the final results would be based on the other 75%, so the final standings may be different.

* Next steps is to understand why XBoost is superior in the regression task. 

* Also I would like to have closer look at outlier analysis, the impact of outliers and how different algorithms deal with it (impact on prediction accuracy)

* An interesting concept to consider is using Bayesian optimization when doing hyper-parameter selection. See Jupyter notebook [here](https://github.com/andriescoetsee/my_first_kaggle_competition/blob/be4682e42d556822c46e966cee80071e86ca62b8/tutorial-bayesian-optimization-with-xgboost.ipynb).

* Furthermore, I would like to learn more about [feature engineering](https://www.kaggle.com/learn/feature-engineering).

#### Finally, in the competition the RMSE differences became marginal between the top 10 where the differentiators were feature engineering and hyper-parameter optimization.








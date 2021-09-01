# [30 Days of ML](https://www.kaggle.com/c/30-days-of-ml)

![image](https://user-images.githubusercontent.com/34986276/130677626-5ac832fb-ba23-4f43-b621-ce999df4e3e4.png)
![image](https://user-images.githubusercontent.com/34986276/131709426-c83fab26-6e78-4ae6-a89c-3a36a6820f33.png)

30 Days of ML on Kaggle was an in class prediction competition on a regression task.

First, I used the Random Forest Regression algorithm. 
I was very much constraint in performance using only CPU for processing (algorithm does not use GPU).
So I had to limit the dataset in order to complete training runs. This adversely affected results. 

[See RandomForest code here](https://github.com/andriescoetsee/my_first_kaggle_competition/blob/4921edfc802a2aa1c968ae869392150fbf53ad9f/30-days-of-ml-random-forest.ipynb)

Then, I tried out the XGBoost algorithm using the same framework. However, this time utilization the full dataset of 300,000 observations for training.
This algorithm utilizes GPU, what a pleasure it was to train the model, adjust parameters, retrain and then seeing how the RMSE (root mean squared error as loss metric) descreases. 

[See XGBoost code here](https://github.com/andriescoetsee/my_first_kaggle_competition/blob/f7237fce1afbd4183cc4e49d1a595238cee49315/30-days-of-ml-xgboost.ipynb)

## Conclusion

At the time of submission the #1 position produced a RMSE of 0.71533 while my own score came in at #2311 with RMSE 0.71781. 
In total there were 7,573 participants. 

![image](https://user-images.githubusercontent.com/34986276/131710214-2a908a25-c85d-47f2-8aa6-75ec6f84261f.png)

* Next steps is to understand why XBoost is superior in the regression task. 

* Also I would like to have closer look at outlier analysis, the impact of outliers and how different algorithms deal with it (impact on prediction accuracy)

* An interesting concept to consider is using Bayesian optimization when doing hyper-parameter selection. See Jupyter notebook [here](https://github.com/andriescoetsee/my_first_kaggle_competition/blob/be4682e42d556822c46e966cee80071e86ca62b8/tutorial-bayesian-optimization-with-xgboost.ipynb).

* Furthermore, I would like to learn more about [feature engineering](https://www.kaggle.com/learn/feature-engineering).

##### Finally, in the competition the RMSE differences became marginal between the top 10 where the differentiators were feature engineering, hyper-parameter optimization and ensemble combinations (stacking of predictors). 








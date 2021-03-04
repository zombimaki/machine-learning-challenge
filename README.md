# machine-learning-challenge

## RandomForest.ipynb

In the RandomForest model notebook we perform the following:
1. Load the exoplanet csv into a dataframe.
2. Created a df of selected feaures without the koi_disposition and koi_tce_plnt_num columns. These will be our x values.
3. Assign koi_disposition to the y vlaue.
4. Split the data with a .35 test size.
5. Scale the data
6. Train the model using the RandomForest classifer and an n_estimators of 500
7. Display the feature names and sort by importance (top will be used in the Logisitc Regression).
8. Print a classification report
9. Perform hyperparater tuning with GridSearchCV
10. Generate the best params and best score.
11. Save the model.

## LogisticRegression.ipynb
In the Logisitc Regression model we perform the following:
1. Load the exoplanet csv into a dataframe.
2. Created a df of selected feaures based on the results of the RandomForest top features.
3. Assign koi_disposition to the y vlaue.
4. Split the data with a .35 test size.
5. Scale the data
6. Train the model using the LogisticRegression classifer with the newton-cg solver and max_ter of 1000.
7. Generate Predictions
9. Perform hyperparater tuning with GridSearchCV
10. Generate the best params and best score.
11. Save the model.


The results of the models were close with the best score of the Random Forest being and the best score of the Logisict Regression being 87%. However the Random Forest prived more useful by being able to tell me the colums that were making the most impact which i could use when building other models.
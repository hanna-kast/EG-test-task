Task:
1. Build a model that predicts "charges" for a given person based on their features.
2. Evaluate the quality of your model.
3. Identify the factors with the highest impact.

Expected result - link to a GitHub repo with:
1. Code for the solution (any programming language, Python or R preferred).
2. Brief summary of the solution*: what did you do, which steps did you make, how to interpret the results.

STRATEGY

1. Checked dataset for missing values and data outliers.
2. Processed nominal variables for correct nodel work (used dummy variables and LabelEncoder).
3. Checked correlation plot for multicollinearity.
4. Splitted dataset for testing and training.
5. Selected 3 models (linear regression, random forest, catboost) to choose the best one.
6. Compared the score of MSE and R2 to see the best model (it's catboost).
7. Did hyperparameter optimization, implemented new parameters which led to a better score.
8. Found the most important features.

CONCLUSIONS

1. The best model is catboost with depth=6, eval_metric='R2', iterations=50, learning_rate=0.1.
2. The model showed MSE = 18394951.461915728 and R2 = 0.8815130321184591.
3. Features with the biggest impact are 'smoker', 'bmi', 'age'.

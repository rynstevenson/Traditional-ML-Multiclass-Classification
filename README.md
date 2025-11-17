# Traditional-ML-Multiclass-Classification
Multiclass classification task. Data was very ambiguous, so data cleaning, EDA, and feature engineering was extensive. This task required a 90/10 split and that I prioritize accuracy as my main performance metric.

I was provided this data with few instructions or context given: I just needed to predict the label column using a 90/10 split, maximizing accuracy. Upon investigation, I discovered the label column had 6 unique values, so this project became a multiclass classificationt task.

I went column by column, performing EDA and engineering features to extract the most meaningful and interpretable information I could. This process also helped me decide on which models to try (random forest, XGBoost, LightGBM). I then looked at feature importance and multicollinearity to narrow down the features I used. After this, I used 5-fold cross validation and a random grid search to select optimal hyperparameters for each model, then evaluated these finetuned models on the test set. The random forest was the overall best performer, achieving 96% accuracy.

If I had more time to complete this project, here are the changes I would've made:
- Try vectorizing columns 1, 4, and 6
- Experiment with upsampling or SMOTE to better address imbalanced nature of data
- Do multicollinearity check before feature importance so that multicollinearity doesn't distort results of feature importance
- Used Spearman rank correlation instead of VIF scores for multicollinearity to account for nonlinear relationships

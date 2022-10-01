# Credit-Risk-Prediction
Credit default risk is the risk that a lender takes the chance that a borrower fails to make required payments of the loan.

The model has data imbalance. So I have utilized SMOTE algorithm to oversample the data so that F1 score wouldnt be affected. 
I utilized different learning algorithms including KNN, Logistic regression, decision tree, and the popular XGBoost to find the best algorithms, and on top of that, I also implemented RandomizedSearchCV and GridSearchCV to fine tune the hyperparamters and further improve the model.

# Final Discussion
* The XGBClassifier has the best performance with 0.986 AUROC score compared to other three classifiers KNN, Logistic regression, and decision tree using the base model.
* Using RandomizedSearchCV to fast optimize hyperparamters, the model AUROC is improved to 0.9862
* With further fine tuning around those hyperparameters using GridSearchCV, the final best model has a 0.9863 AUROC score.
* The optimal probability threshold for the best model is 0.55 resulting accuracy 0.956.

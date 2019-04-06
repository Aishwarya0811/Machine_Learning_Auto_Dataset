# Machine_Learning_Auto_Dataset

## Data Pre Processing 

Getting Dataset ready for ML 

## Data Preparation and Manipulation.

Missing Value:- Replacing Nan values and how are missing values represented in the dataset.
Exploration of Data by doing group bys, statistics etc

## Data Imputation and Data Transformation.

Replacing all columns with a numerical column in this dataset.
Dropping the unwantescolumns form the dataset based on the inferences made.


## ML Models and Algorithims

1. Linear regression

2. KNN regrssor - best param

3. SGDRegressor - best params

4. Ridge - best param

5. Lasso - feature importance, best param

6. LinearSVR - best param

7. SVR kernel = 'rbf' and 'poly' - best params

8. Decision Tree Regressor - best params

## Classification Machine Learning Models

- Train a KNeighborClassifier on this dataset. Which value of the hyper parameter n_neighbors results in an overfitting problem.

neighbors = [1, 5, 10, 15, 20]


- Train a LinearSVC model on this dataset. Fine tune this model by changing the hyperparameter C in [0.01, 0.1, 1, 10]. What can we say about this model. (set random_state = 0)


- Consider Xt = X_train[['age','education-num']][:100], and yt = y_train[:100]. We have the following plots to show decision boundary of SVC(kernel = 'rbf'). Which plot suggest the largest value of C and gamma?  C and gamma in [0.1, 1, 10]. random_state = 0


- Train a LogisticRegression model. Among values C in [0.1, 1, 10] and penalty in ['l1', 'l2'], which combination will give the best fit? (set random_state = 0)


- Train a DecisionTreeClassifier model on this dataset. Which max_depth in  [1, 2, 3, 5, 10] is the best fit? (choose the value that both train and test scores are high and gap between train and test score is small. Set random_state = 0).


- Consider the max_depth in the previous question. Which feature is the most important feature?



## Model evaluations

Question 1:

What is the ratio of label 1 to label 0? (consider two significant digits)

Question 2:

Consider the following scenario: Government is securing a budget for low-income assistance programs. Assume this program will help low-income individuals/families with a fixed rate financial support. We need to have a good model to predict how many individuals/families are eligible for this assistance program. Beside accuracy which evaluation model should we use?

' <=50K':0 - Negative
' >50K':1  - Positive

Question 3 and 4:

Train a LogisticRegression model on this dataset. Set the hyper-parameters as follow:

penalty = 'l1'
random_state = 0
What is the train and test precision score? (with two significant digits)

Question 5 and 6:

Train a dummy classifier that classifies everything as the majority class of the training data. What are the train and test accuracy of this classifier? (numbers with two significant digits)

Questions 7:

Train a LogisticRegression model on this dataset. Set the hyper-parameters as follow:
penalty = 'l1'
random_state = 0
What is the precision score when using a threshold of -2 on the decision function. Use X_test and y_test. (2 significant digits)



## Ensemble learning

Question 1

First train the following models on X_train and y_train.

Linear support vector machine with default parameters.
decision tree with max_depth = 3
K neighbors classifier with n_neighbors = 5.
In the all above models, set random_sate = 0. Compute the test precision score of hard-voting classifier? (two significant digits)

Question 2

First train the following models on X_train and y_train.

Support vector machine with kernel 'rbf' and default parameters.
Decision tree with max_depth = 3
Logistic regression with default parameters.
In the all above models, set random_sate = 0. Compute the test recall score of soft-voting classifier? (two significant digits)

Question 3

Train a bagging classifier on base model logistic regression with default parameters. Set the hyper-parameter as follow:

n_estimators = 100
max_samples = 500
max_features = 5
random_state = 0
What is out of bag score? (two significant digits)

Question 4

Use a grid search to find the best parameters of a random forest machine learning model on this dataset.

max_depth in [1, 3, 5, 7]
max_features in [5, 7, 9]
n_estimators in [100, 200, 500]
random_state = 0
cv = 5
What are the best parameters of the model?

Question 5 

Train a random forest machine learning model on this dataset using the best parameters in the previous question.
#Which feature has the highest importance?

Question 1

We would like to use Ada Boost method to improve the result of a KNeighborsRegressor model with n_neighbors = 5. Use a grid search to find the best parameters of AdaBoostRegressor.

    n_estimators in [10, 50, 100]
    learning_rate in [0.1, 0.5, 1]
Set random_state = 0 if the model has hyperparameter random_state.

What are the best parameters of this model?

Question 2

Train an Adaboost model with the best parameter found in the previous question. What is grid search test score? (two significant digits).

Use random_state = 0

## Dimensionality reduction

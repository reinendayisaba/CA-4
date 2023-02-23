# CA-4
**A brief description of the purpose of the program and what it is doing.**

This program uses a dataset with a total of 48,842 instances that represents the salaries of people together with seven demographic variables to train different ensemble models, including Random Forest Model, AdaBoost, Gradient Boosting, and XGB classifiers. The dataset contains two target classes labeled as 1 and 0, representing “>50k” and “<=50k”.  To ecaluate the accuracy and AUC values of each classifier a range of n_estimator values is used. The program records the best accuracy and AUC values for each of the four models in a table. Before building and training the models, the dataset is analyzed for any missing values, and the variables are encoded to make them usable by the models. The sklearn.ensemble module is used to import  “RandomForestClassifier”, “AdaBoostClassifier”, “GradientBoostingClassifier” algorithm and the “xgboost” library is imported as well. It’s worth noting that for determining the accuracy and AUC values in this program, the n_estimator is the only hyperparameter that changes while all other hyperparameters are kept at default. The different accuracy and AUC values are used to plot two graphs – accuracy vs n_estimator and AUC vs. n_estimator. Finally, for each of the models, two main questions are answered. First, the observations about the classifier’s behavior with respect to the number of estimators. Second, whether there is an optimal value of the estimator within the given range. 

**The Needed libraries, modules, and classes**

There are a few libraries, modules, and classes that need to be imported to be able to run the code:
* The Numpy library needs to be imported to allow mathematical and scientific computations in Python.
* The Pandas library is needed for data manipulation, analysis, and exploration.
* Matplotlib is imported and used for visualizing the accuracy vs n_estimator curves and AUC vs. n_estimator curves.
*	The “OneHotEncoder” and “LabelEncoder” classes are imported from the sklearn.preprocessing module of the skicit-learn library in Python to convert the categorical variables into numerical variables so they can be changed to the appropriate data type for the algorithms.
*	The “RandomForestClassifier”, “AdaBoostClassifier”, and “GradientBoostingClassifier” classes are imported from the “ensemble” module of the Scikit-learn library so that each of the models can be built and trained.
*	The “xgboost” library is imported to be able to build and train the XGBoost model using XGBClassifier. 
*	The accuracy_score, and roc_auc_score functions are imported from the “sklearn.metrics” module to calculate the accuracy and AUC values for the models.

**How to install and run the code along with datasets to be able to run the program successfully.**

To be able to install and run the code successfully, the dataset must be read as a csv file into the notebook and all the needed libraries and modules need to be installed/imported. Each block of code must also be run individually and in a sequential order (one after another). 

**Acknowledgement**

The path used to access the data was provided by Prof. Arin Brahma (GitHub username: ArinB) using the link "https://github.com/ArinB/MSBA-CA-03-Decision-Trees/blob/master/census_data.csv?raw=true". 


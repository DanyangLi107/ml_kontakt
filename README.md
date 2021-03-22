# Machine learning for KONTAKT project (ML_KONTAKT)
This is a machine learning model integrating detailed clinical and genetic information to predict the outcome of social skills intervention in ASD. All data were acquired from the KONTAKT clinical trial. Paper is coming soon. 

## Model strategy
We performed nested cross-validation by splitting whole data into training and validation sets using outer cycle (10-fold) and then splitting the training set again into training and test data using inner cycle (5-fold). Linear support vector machine (SVM), logistic regression and non-linear SVM (radial basis functions (RBF) kernel) were tested for outcome prediction. For feature selection, average coefficient of each feature was calculated using logistic regression, and recursive feature elimination and sequential forward floating selection were implemented in linear and RBF SVM. All models used grid search to determine the best hyperparameters. 


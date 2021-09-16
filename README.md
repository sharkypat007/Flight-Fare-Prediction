# Flight-Fare-Prediction
Flight Fare Prediction Model using Random Forest

I have used a data set that contains the flight fares between different cities in India. It has been subsequently used for Predicting the flight fares between cities.


Section 1- Importing the Libraries- The PYTHON Libraries that have been used have been imported 

Section 2- Importing the Dataset
•	Dataset is an excel file we have imported the data in a Pandas dataframe
•	The Null values (if present have been appropriately treated)

Section 3- Exploratory Data Analysis
•	EDA is performed on the data
•	From description we can see that columns like (Date_of_Journey) are object data type and it is thus converted to timestamp columns so as to use this for prediction
•	Similar extraction is done for other variables.
•	Post Extraction the columns which are of no use anymore are dropped

Section 4- Categorical Data Encoding
•	Nominal data are the data which do not have any order and hence OneHotEncoding is used
•	Ordinal data are the ones which have a specific order to be maintained and hence LabelEncoder is used.

Section 5 - Test Set Data Preprocessing 
Similar steps of data pre-processing were carried out for the test set data as well.

Section 6 - Feature Selection 
 Only those features which will contribute towards the target variable are taken. These features have a good relation with regards to a target variable. 
•	Heat map plotting was done
•	Extract trees regressor was used to select important features 
•	Plotting of the selected features was done

Section 7 - Fitting of model using Random Forest 
•	Train test split was done for prediction with respect to X_test.
•	A scaling is not required for random forest
•	Model import and fitting
•	Prediction with respect to X_test 
•	RMSE score checking and graph plotting

Section 8 – Hyperparameter Tuning
•	RandomizedSearchCV was used for choosing the best hyperparameters for the given model.
•	The best parameters were evaluated and printed
•	Model was fit for best Hyper Parameters and the best score was evaluated
 
Section 9 – Pickling of Model and Final Model Evaluation 
•	Model was saved using pickling and final prediction and performance metrics were evaluated using X_test and Y_test  

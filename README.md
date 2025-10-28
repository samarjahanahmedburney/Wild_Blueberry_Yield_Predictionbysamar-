# Wild_Blueberry_Yield_Predictionbysamar
This project aims to predict the yield of wild blueberries based on various factors such as environmental conditions, bee activity, and pollination rates. The analysis involves exploring the dataset, visualizing relationships between variables, and applying several regression models to predict the yield.

#Project Steps:
#Data Loading and Initial Inspection:

Load the dataset WildBlueberryPollinationSimulationData.csv.
Display the first few rows, shape, and information about the dataset.
Check for missing values and duplicates.
#Exploratory Data Analysis (EDA):

Visualize the distribution of numerical features using histograms.
Analyze the correlation between features using a heatmap.
Examine feature importances from the trained models to understand which factors most influence yield.
#Data Preprocessing:

Handle missing values (although none were found in this dataset).
Split the data into training and testing sets.
Scale numerical features for models sensitive to feature scaling (like SVR).
Model Training and Evaluation:

Train several regression models:
Linear Regression
Decision Tree Regressor (with GridSearchCV for hyperparameter tuning)
Random Forest Regressor
XGBoost Regressor
Support Vector Regressor (SVR) (with GridSearchCV for hyperparameter tuning)
Evaluate each model using metrics such as RMSE, MAE, and R².
Model Comparison:

Compare the performance of the trained models based on the evaluation metrics.
Visualize the comparison using bar plots and line plots.
Results:
The model comparison revealed the following performance metrics:

Model	RMSE	MAE	R²	RRMSE
XGBoost	131.24	104.51	0.99	2.24
Linear Regression	17819.14	99.42	0.99	2.27
Random Forest	22592.09	113.66	0.99	2.56
SVR	23890.70	117.82	0.99	2.63
Decision Tree	44234.11	145.28	0.98	3.58
Based on the RMSE, the XGBoost model performed the best on this dataset.

Feature Importance:
(Include the feature importance plots generated in the notebook)

The feature importance analysis from the Decision Tree and XGBoost models indicates that fruitset, seeds, and fruitmass are the most influential factors in predicting wild blueberry yield.

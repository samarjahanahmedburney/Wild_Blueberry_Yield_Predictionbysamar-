# Wild_Blueberry_Yield_Predictionbysamar
This project aims to predict the yield of wild blueberries based on various factors such as environmental conditions, bee activity, and pollination rates. The analysis involves exploring the dataset, visualizing relationships between variables, and applying several regression models to predict the yield.

**Project Steps:**
**1. Project Title and Description:**

Title: Wild Blueberry Pollination Simulation Model
Description: Briefly explain what the project is about. Mention that it's a simulation model to predict wild blueberry pollination based on various factors like bee activity, environmental conditions, and fruit characteristics.
**2. Objectives:**

Reiterate the main goal of the simulation model, which is predicting pollination.
**3. Libraries and Tools Used:**

List the key libraries you used (NumPy, Pandas, Matplotlib, Seaborn, Scikit-learn, XGBoost, Pipeline, ColumnTransformer). Briefly mention what each library was used for, similar to your "Libraries and Tools Used" markdown cell.
**4. Data Source:**

Mention the dataset you used (WildBlueberryPollinationSimulationData.csv) and where it came from (if it's publicly available, provide a link).
**5. Exploratory Data Analysis (EDA):**

Describe the EDA steps you performed, such as:
Checking the dataset shape, info, and statistical summary.
Identifying missing values and duplicates.
Visualizing data distributions (histograms).
Analyzing correlations between features and the target variable (yield) using a heatmap.
Analyzing key features related to bees and their relationship with yield.
Detecting outliers using boxplots.
**6. Data Preprocessing:**

Explain the preprocessing steps:
Feature-target separation.
Outlier removal using the IQR method.
Identifying and handling highly correlated features (mention which ones were dropped or how they were handled).
Feature grouping for PCA.
Using ColumnTransformer and Pipeline for preprocessing.
**7. Model Development and Evaluation:**
1.Linear Regression
2.Decision Tree Regressor (with GridSearchCV for hyperparameter tuning)
3.Random Forest Regressor
4.XGBoost Regressor
5.Support Vector Regressor (SVR) (with GridSearchCV for hyperparameter tuning)
Evaluate each model using metrics such as RMSE, MAE, and R².
Explain how you created end-to-end pipelines for each model.
Describe the evaluation metrics you used (RMSE, MAE, R²).
Present the model performance summary table and visualizations (barplot and line plot) comparing the models based on their RMSE.
Highlight the best-performing model(s) based on your evaluation.
**8.Model Comparison:**

Compare the performance of the trained models based on the evaluation metrics.
Visualize the comparison using bar plots and line plots.
Results:
The model comparison revealed the following performance metrics:
**Model Performance Summary:**
   **Model**          **	RMSE**     **	MAE**    **	R²**
0	Gradient Boosting  	123.540374  	97.087767	 0.992148
1	XGBoost	            149.909630 	117.766398 	0.988438
2	Random Forest      	152.033741 	111.688121 	0.988108
3	Linear Regression  	165.531590	 123.386471	 0.985902
4	Decision Tree	      184.044687	 140.036304 	0.982573

Based on the RMSE, the XGBoost model performed the best on this dataset.

**9.Feature Importance:**
(Include the feature importance plots generated in the notebook)

The feature importance analysis from the Decision Tree and XGBoost models indicates that fruitset, seeds, and fruitmass are the most influential factors in predicting wild blueberry yield.

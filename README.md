# Forecasting-Churn-Azure-vs.-Traditional-ML-at-ABC-Telecom
Championing Accuracy: Azure AutoML outperforms manual methods across XGBoost, Random Forest, and Logistic Regression algorithms in predicting churn at ABC Telecom

![image](https://github.com/TheRonnie/Forecasting-Churn-Azure-vs.-Traditional-ML-at-ABC-Telecom/assets/98576788/57fe65f1-e048-4778-afb6-6bfbdf71b76a)


Unleashing Predictive Power with Azure Cloud for Churn Prediction at ABC Telecom
● Examined customer data using Azure Cloud to find clues about who might stop using ABC Telecom.
● Used Azure tools like Databricks and AutoML to build models that predict if a customer will leave.
● Made better predictions (14% better!) than before, helping ABC Telecom keep more customers happy by giving them 
what they need before thinking about leaving

### Tasks – Manual Prediction:
1.	Data Pre-processing (1/3):

        •	Converted all FLOAT values to 2 decimal places.
        •	Converted Date OBJECT columns to DATETIME format.
        •	Identified and handled columns with high null values (>20%).
        •	Replaced null values in continuous columns:
              1.	NUMBER columns replaced with '0'.
              2.	CATEGORICAL columns replaced with 'NA'.
        •	Dropped high null value Date columns.

2.	Data Pre-processing (2/3):
        
        •	Treated null values for derived columns.
        •	Identified and dropped columns with nil variance.
        •	Identified High-Value Customers based on 70th percentile of average recharge amount.

3.	Data Pre-processing (3/3):

        •	Identified churn count for the 9th month (churn phase).
        •	Dropped null value rows.
        •	Exported remaining non-null rows.

4.	Exploratory Data Analysis (1/3):

         •	Univariate analysis (Hist. plot) revealed similar data distribution for each month.

5.	Exploratory Data Analysis (2/3):
      
        •	Bivariate analysis (Pair plot) showed correlation between variables.
        •	Bivariate analysis (Heat-map) depicted the magnitude of correlation between variables.

6.	Exploratory Data Analysis (3/3):

        •	Bivariate analysis (Violin plot) confirmed balanced data class.


7.	Data Modeling:
        
        •	Treated dataset for outliers (0.01-0.99 quantile).
        •	Defined target column.
        •	Split dataset into test and train sets.
        •	Separated target column.
        •	Scaled the variables.

### Steps for Azure AutoML:

1.	Storage – Azure Data Lake:

        •	Ingested .csv file into Azure Data Lake.
        •	Pre-processed .csv file stored and exported into Azure Data Lake.

2.	Data Processing – Azure Databricks:

        •	Data imported into Azure Databricks for processing.

3.	Model Training – Azure ML:

        •	AutoML model pipeline created in Azure ML.
        •	XGBoost classifier selected as the best model with a prediction accuracy of 0.953.

4.	Deploy Model as Web App:

        •	Model deployed as a web service for accessibility.

5.	Comparison of Prediction Accuracies:

	XGBoost Classifier:

        •	Employed Manually: 0.834
        •	AutoML: 0.953

	Random Forest:

        •	Employed Manually: 0.781
        •	AutoML: 0.951

	Logistic Regression:

        •	Employed Manually: 0.810
        •	AutoML: 0.945

## Azure AutoML consistently outperformed manual employment across all algorithms, with the XGBoost classifier providing the best prediction accuracy of 0.953.



###

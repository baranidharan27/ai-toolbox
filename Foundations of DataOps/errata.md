#### List of code errate

# The DataOps Lifecycle

#### 1.1 DataOps pipeline for ML model training

Synthetic data has been added to the provided code in the textbook . This generates synthetic customer data for a churn prediction scenario. It creates a dataset with 1000 samples, including customer tenure, two random features, and a binary churn indicator.

#### 1.1 CI/CD pipeline with Git and DVC

In the textbook, a basic CI/CD workflow using Git and DVC has been implemented, showcasing how code, data, and model versions can be managed and deployed in a DataOps context. The implementation sets up a Git repository, initializes DVC, creates placeholder dataset and model files, and tracks them with Git and DVC. It then performs simple steps for running tests and deploying. 

#### 1.1 Agile DataOps sprints

Each function is a placeholder for a specific task and hence created , added along with the code mentioned in the textbook.  

#### 1.1 role interactions in a DataOps project
Each function is a placeholder for a specific task and hence created , added along with the code mentioned in the textbook.





# Automation collaboratioon and monitoring 


#### 1.1 Automated data pipeline with error handling



**CHANGES:** prefect has updated its API new version is **flow** using this ensure run on google colab with the older version i got error the difference is prefect 1.x (old) now changed into prefect 2.x (new)

**Error handling:**
changed into centralized error handling using  **execute_task** its ensure the DRY and it works fine



#### 1.1 Basic monitoring in a data pipeline
**Change:**
-Prefect has updated its API, and the newer version uses flow instead of Flow

#### **Result Handling:**
- The use of LocalResult for result handling is not necessary for basic tasks. Prefect handles results efficiently by default, 
    

#### **Transformation Logic:**

**change:**

- The proposed code includes additional transformations (numeric_squared and float_rounded), providing a transformation process. It also removes the unnecessary Local Result and defines the some_transformation function for clarity.
    
    
#### **Data Quality Monitoring:**

**Change:**
 The proposed code includes additional quality checks for the new columns (numeric_squared and float_rounded), ensuring comprehensive data quality monitoring.

####  **Flow Definition and Execution:**
**Change:**
 Using the @flow decorator provides a clearer and more concise way to define the flow. It also aligns with the modern Prefect API, 


#### 1.2 Simple example of how structured data might be represented and processed

#### **Test_train_split :**
**Changes:** Adding 'random_state=42' ensure the reproducibility and ensure the split eill be same everytime you run the code.


#### 1.2 Simple example of processing unstructured text data:

      NO CHANGES 



#### 1.2 example of working with semi-structured data in JSON format:
    
      NO CHANGES


# Data collection and ingestion strategies


#### 1.2 Batch data ingestion process using python 

Synthetic data has been added to the provided code in the textbook

**Change:**
Used SQLite data base since no need for database credentials or network setup.We can also use PostgreSQL



#### 1.2 Real-time data streaming using Python and Kafka

**Change:**
It is assumed the local host for Kafka engine is setup by the user

#### 1.2 API- based data collection using python
      NO CHANGES


#### 1.2 Webscrapping using python
      NO CHANGES

# Datapreprocessing and quality assurance

#### 1.2 data cleaning techniques

      NO CHANGES

#### 1.2 Handling Missing data

df[column] = np.round(imputer.fit_transform(df[[column]]),1) ## Put np.round for consistency accross the whole data np.round rounds off to the decimal value specified

#### 1.2 Data normalization and standardization 
      NO CHANGES
#### 1.2 Data Quality metrics and validation

Original if pd.api.types.is_numeric_dtype(df[column]): elif pd.api.types.is_string_dtype(df[column]) Corrected if pd.api.types.is_numeric_dtype(column): elif pd.api.types.is_string_dtype(column):

Passing as a column of the pandas dataframe results in keyerror. Instead pass it as Pandas Series


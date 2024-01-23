# DATA SCIENCE PROJECT REPORT ON PORTUGUESE BANK MARKETING 
## BUSINESS CASE: BASED ON THE GIVEN FEATURE OF DATASET WE NEED TO CREATE PREDICTIVE MODEL WHICH HELP BANK MARKETING TEAM TO KNOW WHICH CUSTOMER WILL BUY PRODUCT (BANK TERM DEPOSIT).

### Abstract:
The aim of this marketing research project is to develop a robust classification model using machine learning techniques to analyse and enhance the marketing strategies of a Portuguese bank. The goal is to attract new customers, improve customer engagement, and increase subscription for term deposit services. The research focuses on understanding customer behaviour, preferences, and perceptions related to direct marketing campaigns (phone calls) of a Portuguese banking institution. The specific classification objective is to predict whether a client will subscribe to a term deposit (variable Target). 
Methodology involves data preprocessing, exploratory data analysis (EDA), feature engineering, and the application of machine learning algorithms. to figure out which customers might be interested in the bank's services based on their details like contacts, social and economic background, and other important information. We used specific techniques like classification algorithms to do this.
 

### Device Project In-to Multiple Steps:
1.	Data Collection 
1.	2.Loading data
2.	3.Domain Analysis 
3.	4.Basic Checks of data
4.	EDA (Univariate, Bivariate, Multivariate Analysis)
5.	Data Pre-processing 
6.	Feature Selection 
7.	Building ML Model
8.	Training & Model Evaluation
9.	Model Savings

### Loading data:
load data in python using panda’s library

### Domain analysis:
#### BANK CUSTOMERS DATA
**1. AGE:**
- This is the different age group of the Account Holder in the dataset.

**2. JOB:**
- This variable probably represents the occupation or job of the customers Knowing this helps us understand their occupation, which can be useful for tailoring marketing efforts.

**3. MARITAL:**
- This variable likely represents the marital status of the customers such as "single", "married" or "divorced."

**4. EDUCATION:**
- This could represent the educational level of the customers like "high school", "college" or "university."

**5. DEFAULT:**
- This might be a binary variable indicating whether the customers have defaulted on a financial obligation or not.

**6. HOUSING:**
- This could be a binary variable indicating whether the customers has a housing loan or not.

**7. LOAN:**
- This might be a binary variable indicating whether the customers have a loan or not.

#### RELATED WITH THE LAST CONTACT OF THE CURRENT CAMPAIGNS

**8. CONTACT:**
- This variable probably represents the method of contact used to reach out to these customers which could include "cellular" "telephone" or "unknown".

**9. MONTH:**
- This likely represents the month when the last contact was made possibly useful for seasonal analysis.

**10. DAY_OF_WEEK:**
- Day of the week of the last contact made with the person. This provides information about the timing of the communication or marketing efforts.

**11. DURATION:**
- This might represent the duration of the last contact with the customers in seconds.

#### OTHER ATTRIBUTES

**12. CAMPAIGNS:**
- It represents the number of marketing campaigns or contacts made with customers during the current effort.

**13. PDAYS:**
- This could represent the number of days since the customers was last contacted possibly related to a previous marketing campaign.

**14. PREVIOUS:**
- This variable might represent the number of contacts performed with the customers before this current campaign.

**15. POUTCOME:**
- It represents the outcome of previous marketing campaigns, whether they were "successful" "failure" or "nonexistent".

#### SOCIAL AND ECONOMIC CONTEXT ATTRIBUTES

**16. EMP.VAR.RATE: (EMPLOYMENT VARIATION RATES)**
- Employment variation rate quarterly indicator. This is an economic indicator that reflects changes in the employment market.

**17. CONS.PRICE.IDX: (CUNSUMERS PRICE INDEX)**
- Consumer price index monthly indicator. This is a measure that examines the average change in prices paid by consumers for goods and services over time, indicating inflation or deflation trends.

**18. CONS.CONF.IDX: (CONSUMERS CONFIDENCE INDEX)**
- Consumer confidence index monthly indicator. This measures the degree of optimism on the state of the economy that consumers are expressing through their activities of savings and spending.

**19. EURIBOR3M: (EURIBOR 3-MONTH RATE)**
- Euribor 3-month rate daily indicator. This is the interest rate at which European banks lend funds to one another for a three-month period in the Eurozone.

**20. NR.EMPLOYED: (NUMBER OF EMPLOYEES)**
- Number of employees quarterly indicator. This represents the quarterly average number of employed people.

#### OUTPUT FEATURE

**21. TARGET:**
- This is the target variable. It indicates whether a customers has subscribed to a term deposit. It's typically a binary choice, with "yes" or "no".

### EDA (Univariate, Bivariate, Multivariate Analysis)
#### I.	Univariate Data Analysis
Use sweetviz library and generate a html report of all feature to do univariate analysis, in that we get the Minimum, Maximum, Some statistical information of the particular feature.

#### II.	Bivariate Data Analysis
In Bivariate analysis we check the relation of independent features to each other.

#### III.	Multivariate Data Analysis¶
In multivariate analysis we check the correlation of two independent features to each other.

### Data Preprocessing
•	First, we check the missing values, but in this data, there is no missing values present.
•	Second, we Handle categorical data and use Manual encoding and frequency encoding. Because features have contained lots of label.
•	In this data I’m Clearly seen that some feature has lots of outlier & we impute them, for that first we check the distribution of all feature and plot the box plot and decide the technique. In this data we are handle feature outlier, 
•	Scale the numerical independent feature with the help of Standard scalar and scale the feature. Because standard scaling gives me the best result of ML model.

### Feature Engineering
•	Check the correlation with the help of heatmap and seen the from the above heatmap is very difficult to find highly correlated feature so we are creating a python code to check the highly corelated feature and drop highly correlated feature. 
•	The dataset has 29 duplicate values.
•	After that save & load the preprocess data, Save the dataframe to a CSV file.

### Model Creation & Evaluation
•	Define Independent and dependant variable and split the data into training and testing.
•	For Training 80% & Testing 20% data
•	I check data is balanced or not after check the data has imbalanced so I utilized the SMOTE technique to balance the data.
•	Use classification algorithm algorithms including Logistic Regression, Decision Tree, Random Forest, XGBoost, KNN, and Artificial Neural Network (ANN).
•	Afterward, I evaluated the models using accuracy, recall, precision, and F1 score metrics.

#### Best model
Our best performed model with accuracy (0.90) metric is XG Boost and Logistic. This classifier could achieve accuracy rate 0.90 that is average accuracy.

### Model Saving 
·	Save the model using pickle file.

### Conclusion
•	This analysis can be carried out at the level of individual bank branches as does not require much resources and special knowledge (the model itself can be launched automatically with a certain periodicity).
1.	Take into account the time of the company (May is the most effective)
2.	The model shows that students and senior citizens respond better to proposal.
3.	profession accurately determine the marketing profile of a potential client.
4.	the bank’s contact time with the client - it affects most of all on conversion.
•	Given these factors, it is recommended to concentrate on those consumer groups that are potentially more promising.
•	Many banks use direct marketing strategies to enable customers to access adequate information about the products. Researchers suggest that the applicability of data mining techniques depends on the availability of customers’ information. Also, studies reveal that machine learning techniques determine customer response to bank products.
•	The ability of the customers to subscribe to term deposits depends on the marketing campaign by the bank. In this research work three machine learning algorithms (Logistic regression, Decision Tree, Random Forest, XGB Classifier, KNN, ANN) were deployed to find out the main factor that influences customers decision to subscribe to a term deposit in the bank. Correlation heatmap was then used to get the most important factors that influence customer decisions and was then retrained to perform the

-------------------------------------------------------------------Thank You-------------------------------------------------------------------






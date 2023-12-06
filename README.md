# Logistic Regression in Bank Marketing Dataset

## Dataset Information
| **Dataset Characteristics** | Multivariate               |
|-----------------------------|---------------------------|
| **Subject Area**            | Business                  |
| **Associated Tasks**        | Classification            |
| **Feature Type**            | Categorical, Integer      |
| **Number of Instances**     | 41199                     |
| **Number of Features**      | 20                        |


## Dataset Columns

#### Bank Client Data
1. **age (numeric)**
2. **job**: Type of job (categorical: 'admin.','blue-collar','entrepreneur','housemaid','management','retired','self-employed','services','student','technician','unemployed','unknown')
3. **marital**: Marital status (categorical: 'divorced','married','single','unknown'; note: 'divorced' means divorced or widowed)
4. **education**: Education level (categorical: 'basic.4y','basic.6y','basic.9y','high.school','illiterate','professional.course','university.degree','unknown')
5. **default**: Has credit in default? (categorical: 'no','yes','unknown')
6. **housing**: Has housing loan? (categorical: 'no','yes','unknown')
7. **loan**: Has personal loan? (categorical: 'no','yes','unknown')
#### Related with the Last Contact of the Current Campaign
8. **contact**: Contact communication type (categorical: 'cellular','telephone')
9. **month**: Last contact month of the year (categorical: 'jan', 'feb', 'mar', …, 'nov', 'dec')
10. **day_of_week**: Last contact day of the week (categorical: 'mon','tue','wed','thu','fri')
11. **duration**: Last contact duration, in seconds (numeric). Important note: this attribute highly affects the output target (e.g., if duration=0 then y='no'). Yet, the duration is not known before a call is performed. Also, after the end of the call y is obviously known. Thus, this input should only be included for benchmark purposes and should be discarded if the intention is to have a realistic predictive model.
#### Other Attributes
12. **campaign**: Number of contacts performed during this campaign and for this client (numeric, includes last contact)
13. **pdays**: Number of days that passed by after the client was last contacted from a previous campaign (numeric; 999 means the client was not previously contacted)
14. **previous**: Number of contacts performed before this campaign and for this client (numeric)
15. **poutcome**: Outcome of the previous marketing campaign (categorical: 'failure','nonexistent','success')
#### Social and Economic Context Attributes
16. **emp.var.rate**: Employment variation rate - quarterly indicator (numeric)
17. **cons.price.idx**: Consumer price index - monthly indicator (numeric)
18. **cons.conf.idx**: Consumer confidence index - monthly indicator (numeric)
19. **euribor3m**: Euribor 3-month rate - daily indicator (numeric)
20. **nr.employed**: Number of employees - quarterly indicator (numeric)
#### Output Variable (Desired Target)
21. **y**: Has the client subscribed to a term deposit? (binary: 'yes','no')

## Learning Outcomes
- Exploratory Data Analysis
- Data Preparation for Model Training
- Model Training using Logistic Regression
- Model Performance Comparison

## Objective
The primary classification goal is to predict if the client will subscribe (yes/no) to a term deposit (variable y).

## Steps and Tasks
1. **Import the necessary libraries**
2. **Read the data as a data frame**
3. **Perform basic EDA**
   - Shape of the data
   - Data type of each attribute
   - Checking the presence of missing values
   - 5-point summary of numerical attributes
   - Checking the presence of outliers
4. **Prepare the data to train a model**
   - Check if data types are appropriate
   - Handle missing values
5. **Train the model with logistic regression module**
   - Note and comment on performances along different metrics

## About the Dataset
### Abstract
The data is related to direct marketing campaigns (phone calls) of a Portuguese banking institution. The classification goal is to predict if the client will subscribe a term deposit (variable y).
### Information
The dataset comprises direct marketing campaigns conducted by a Portuguese banking institution, based on phone calls. The goal is to predict whether the client will subscribe to a term deposit (variable y). The marketing campaigns span from May 2008 to November 2010.
### Acknowledgements
This dataset is publicly available for research and was analyzed in [Moro et al., 2014]. Please cite the following if you use this database:
[Moro et al., 2014] S. Moro, P. Cortez and P. Rita. A Data-Driven Approach to Predict the Success of Bank Telemarketing. Decision Support Systems, Elsevier, 62:22-31, June 2014

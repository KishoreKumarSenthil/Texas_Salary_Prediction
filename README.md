# Texas_Salary_Prediction

# Problem Statement:
Task 1 :- Prepare a complete data analysis report on the given data.

Task 2 :- Create a predictive model which will help the Texas state government team to know the payroll information of employees of the state of Texas.

Task 3 :- Who are the outliers in the salaries?     
What departments/roles have the biggest wage disparities between managers and employees?    
Have salaries and total compensations for some roles/ departments/ head-count changed over time?

# Project Summary :
- This database has salary information for positions at all 113 agencies in the Texas state government. The Tribune obtained this data by requesting salary records from the state comptroller, as allowed by the Texas Public Information Act.

- Our main objective is to predict salary information of employees at different agencies in Texas state government using given twenty one features.

- We were able to analyse the salary information and built different models which help us to analyse the dataset properly.We classify the dataset according to the data preparing description. We showed various plots for easy reading and understanding.

- After the EDA, the dataset was preprocessed by using categorical data encoding using LabelEncoder,removing outliers, scaling some numerical columns.

- We take 'agency', 'class_title', 'ethnicity', 'gender', 'status','hr_rate', 'hr_per_wk', 'm_salary', 'state_no' as relevent feature as our input variables and "a_salary" i.e. annual salary as our target variable.

- Performed models are "LinearRegressor", "DecisionTree", "RandomForest", "GradientBoostingRegressor" to be compared by the used of r2score, adjusted r2 score, mse, mae and based on that the linear regressor came out on top.

# There are some of challenges that as a team we face are :
1) Poor Quality of Data:
One of the significant issues our team face is the absence of good quality data. Unclean and noisy data can make the whole process extremely exhausting. There is null values in "duplicated", "comb_mlti_jobs", "summed_annual_salary", "hide_from_search" In many features there is a lack of variation like the standard deviation for "multiple full time jobs" column is 0, means no variance in the data.
to overcome this issue we drop some features because having more then 96% of missing values, we are ignoring those columns.

2) Slow process:
The machine learning models are highly efficient in providing accurate results, but it takes a tremendous amount of time.At the time of exploratory data analysis process it take lot of time when analyse bivariate and multivariate analysis.
So to overcome this issue we did bivariate analysis of relevent featues only.

3) Underfitting of Training Data:
This process occurs when data is unable to establish an accurate relationship between input and output variables.It signifies the data is too simple to establish a precise relationship.
To overcome this issue: Maximize the training time,add relevent features to the data, increasing the training time of model.

4) Overfitting of Training Data:
Overfitting refers to ML model trained with a massive amount of data that negatively affect its performance.
We can tackle this issue by:Analyzing the data with perfection, remove outliers in the training set, remove unwanted feature.
For particular agency_name their will be unique agency_code, so we are droping agency_name and also We dropped last name, first name, MI and emp_date because these are not relevent features for our model creation.

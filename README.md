# customer_churn_large_dataset-Machine-Learning


**Choosing Variable**

Churn  is the dependent variable (y)  and others are independent variables(x).
I have Chosen Churn as Target variable because it is showing the conversion or we can say that how many customers actually continue or discontinue.

**Data preprocessing and cleaning**

 There is no Missing and Duplicate value in this dataset.
Drop column 'CustomerID',  'Name'
**Feature engineering creativity and effectiveness**
. 
 Created  new feature: Usage_per_Month →  df['Usage_per_Month'] = df['Total_Usage_GB'] / df['Subscription_Length_Months']
Standardize numerical features using Standardscaler →'Monthly_Bill', 'Total_Usage_GB', 'Subscription_Length_Months', 'Usage_per_Month'
Done scaling on given column to convert column on the basis of scale for better Accuracy

df["Location"].replace(['Los Angeles', 'New York', 'Miami', 'Chicago', 'Houston'],[1,4,3,2,0], inplace=True)--->
Using this code I have replaced the location name with value using pandas….
Convertec Age into Mean Value.

**Dividing Dataset in Dependent and Independent Data Table**


**Split Data in to Feature and Target Variable**
In x  I have taken 'Monthly_Bill', 'Total_Usage_GB', 'Subscription_Length_Months', 'Usage_per_Month',Age,Gender

**Train Test Split**

Split data in to Test and Train data with test_size of 0.20
Train model with Decision Tree Classifier ,logistic regression,SVC, Random forest

**Classification report**

I have made classification report where i get Precision,Recall,Accuracy,f1 Score .



          


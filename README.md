# Diabetes-Readmission-classification

The project aims at finding out whether a diabetic patient should be readmitted to the hospital or not.

#Dataset

The dataset consisted of data of around 1 lac diabetic patients from around 30 US hospitals collected since 1994-2004.
Data had some missing values and also some string values.

#Data wrangling

1. Missing values were eliminated from the data, which eliminated around 2000 tuples. Then since classification algorithms were to be applied on the dataset to find out the result the string values had to be converted into integer values which was done using One Hot Encoding.

2. Then feature selection was done using Select k best where 4 best attributes were selected, and variance threshold method was used.
Some feature attribute that played a significant rle in predicting the results were:
  'age', 'time_in_hospital', 'num_lab_procedures',
       'num_procedures', 'num_medications', 'number_diagnoses', 'A1Cresult', 'metformin', 'insulin'.
#Algorithms

The algorithms that were applied to predict the result were

1. K Nearest Neighbour
2. Decision Tree
3. Random Forest
4. Support Vector Machines

#Result
The best algorithm that worked with an accuracy of 63% was Decision Tree.

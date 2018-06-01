# BinaryClassification

Type of classification in which target column has two labels is called Binary classification.In this project, 'admit' column (of Admissions.csv ) which is
'1' when student gets an admit 
'0' when student is rejected by university
is to be classified.

## Dataset

Admissions.csv dataset contains data on 644 applicants with the following columns:

1.  gre - applicant's score on the Graduate Record Exam, a generalized test for prospective graduate students. Score ranges from 200 to 800.

2.  gpa - college grade point average. Continuous between 0.0 and 4.0.

3.  admit - binary value. Binary value, 0 or 1, where 1 means the applicant was admitted to the program and 0 means the applicant was rejected.
	
## Logistic function
	
Function is internally used by LogisticRegression model to predict probabilities.It is used because 1)contains exponential term (due to which it is always positive). 2) t/(1+t) form which limits its range from 0 to 1.
	

## Training 

'fit' method of LogisticRegression class is used for training model. It takes two parameters :- 1)'gpa' column (feature)  2) 'admit' column (target)

## Classification

'predict_proba' method of LogisticRegression class is used for predicting probabilities for target column
'predict' method of LogisticRegression class is used for classification (based on threshold (which is 0.5(by default)).

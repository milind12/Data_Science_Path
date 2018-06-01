# BinaryClassification

	Admissions.csv dataset contains data on 644 applicants with the following columns:

	1.  gre - applicant's score on the Graduate Record Exam, a generalized test for prospective graduate students. Score ranges from 200 to 800.
	2.  gpa - college grade point average. Continuous between 0.0 and 4.0.
	3.  admit - binary value. Binary value, 0 or 1, where 1 means the applicant was admitted to the program and 0 means the applicant was rejected.
	
##Logistic function
	
	Function is used internally by LogisticRegression model to predict probabilities.Main characteristics of function is that 1) exponential term (due to which it is always positive). 2) t/(1+t) form which limits its range from 0 to 1.
	


# Predicting-house-prices

## Dataset

Here are some of the columns:

1. Lot Area: Lot size in square feet.

2. Overall Qual: Rates the overall material and finish of the house.

3. Overall Cond: Rates the overall condition of the house.

4. Year Built: Original construction date.

5. Low Qual Fin SF: Low quality finished square feet (all floors).

6. Full Bath: Full bathrooms above grade.

7. Fireplaces: Number of fireplaces.

## Feature Engineering

Goal of feature engineering is to:

1. remove features that we don't want to use in the model, just based on the number of missing values or data leakage

2. transform features into the proper format (numerical to categorical, scaling numerical, filling in missing values, etc)

3. create new features by combining other features


## Feature Selection

Now that we have cleaned and transformed a lot of the features in the data set, it's time to move on to feature selection for numerical features, 

1) We generate a correlation heatmap matrix of the numerical features in the training data set to find whether features correlate strongly with our target column, SalePrice 

2) We calculate the correlation coefficients for the columns that seem to correlate well with SalePrice. 

3) We can remove a categorical column if it has hundreds of unique values (or categories) or it has a low variance. (no variability in the data for the model to capture).



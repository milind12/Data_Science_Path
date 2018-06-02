# predicting-car-prices


## Data Cleaning

1) Missing values in data set must be replaced with np.nan type

2) 'bore','stroke','compression_ratio','peak-rpm','price' columns contain more missing values.So, they can be dropped.

3) 'normalized_losses' contain few missing values. So, null values can be filled with mean of the column.


## Hyperparameter tuning

As k is a parameter which can affect our result, we find its optimum value to minimize error.

## Feature Selection

Most relevant features are selected based on domain knowledge. Some experiments on adding and removal of features also helps.

## Training, testing and cross validation

K Fold class is used to create K folds of dataset and cross_val function is used for crossvalition and average root mean square value is calculated to evaluate the model

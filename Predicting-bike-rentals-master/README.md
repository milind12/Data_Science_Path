# Predicting-bike-rentals

In this project, we predict the total number of bikes people rented in a given hour. We predict the cnt column using all of the other columns, except for casual and registered.

## Dataset

Descriptions for the relevant columns:

1. instant - A unique sequential ID number for each row

2. dteday - The date of the rentals

3. season - The season in which the rentals occurred

4. yr - The year the rentals occurred

5. mnth - The month the rentals occurred

6. hr - The hour the rentals occurred

7. holiday - Whether or not the day was a holiday

8. weekday - The day of the week (as a number, 0 to 7)

9. workingday - Whether or not the day was a working day

10. weathersit - The weather (as a categorical variable)

11. temp - The temperature, on a 0-1 scale

12. atemp - The adjusted temperature

13. hum - The humidity, on a 0-1 scale

14. windspeed - The wind speed, on a 0-1 scale

15. casual - The number of casual riders (people who hadn't previously signed up with the bike sharing program)

16. registered - The number of registered riders (people who had already signed up)

17. cnt - The total number of bike rentals (casual + registered)

## Feature Transformation

'hr' column in bike_rentals contains the hours during which bikes are rented, from 1 to 24. A machine will treat each hour differently, without understanding that certain hours are related. We can introduce some order into the process by creating a new column with labels for morning, afternoon, evening, and night. This will bundle similar times together, enabling the model to make better decisions.

## Applying Linear Regression

We use the LinearRegression class from sklearn to train a machine learning algorithm on train set, then make predictions and calculate error metric.

## Applying Random Forests

Random forests tend to be much more accurate than simple models like linear regression. We use the RandomForestRegressor class from sklearn to train a machine learning algorithm on train set, then make predictions and calculate error metric.

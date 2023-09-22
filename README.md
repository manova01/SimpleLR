# SimpleLR
This is a simple linear regression model 
I did a simple linear regression model using the housing dataset. Only rows which ocean proximity of either <1H OCEAN' or 'INLAND'.
The following columns were used 'latitude',
'longitude',
'housing_median_age',
'total_rooms',
'total_bedrooms',
'population',
'households',
'median_income',
'median_house_value'.
I shuffled the data using seed(42), I split the data into train/val/test sets, with 60%/20%/20% distribution. In which I apply the log transformation to the median_house_value variable using the np.log1p() function.
I filled the missing values for the column with mean and then 0 the RMSE were both good .
I regularisation I used[0, 0.000001, 0.0001, 0.001, 0.01, 0.1, 1, 5, 10] on the validation to see which one does best  Which was 0
I used seed 42 for splitting the data. I wanted to see how seed influence the score , so I tried different seed values: [0, 1, 2, 3, 4, 5, 6, 7, 8, 9].
For each seed, I did the train/validation/test split with 60%/20%/20% distribution, filled the missing values with 0 and train a model without regularization. For each seed, I evaluated the model on the validation dataset and collect the RMSE scores. I wanted to know the standard deviation of all the scores.

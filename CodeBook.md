# CodeBook

ftr:
1. 561 obs. of  2 variables 
2. n(int), function(chr)

act:
1. 6 observations of 2 variables
2. code(int), activity(chr)

x_train:
2947 observations of  561 variables

y_train:
7352 observations of  1 variable

x_test:
2947 observations of  561 variables

y_test:
2947 observations of  1 variable

Data Transformations performed:
1. Merged corresponding train and test sets into X, Y and Subject using rbind(), subject created using cbind().
2. Subject, X and Y merged using cbind() to create Merged_Data.
3. Extract only mean and Standard Deviation into tidy_data; only subject, code, mean, and standard deviation is taken into tidy_data
4. code column in tidy_data replaced with activity from the second column of the activities variable
5. Labelled tidy_data dataset with descriptive variable names
6. final_data is created by summarizing tidy_data via the mean of each variable for each activity and each subject after groupped by subject and activity

## CS6405 - Data Mining

The instructions for the assignment are the following:

### Specification

The objective of this project is to build a k-Nearest Neighbour algorithm that takes as input training and test dataset and will predict the target variable with a reasonable degree of accuracy.

You will find a template for your python code in Canvas along with the dataset. In this project, you must implement your own machine learning library, and therefore you are only allowed to use the following python packages and libraries: NumPy and pandas.

This project focuses on a modified version of the Real estate valuation data set (link). You can find the correct csv here:

https://github.com/andvise/DataAnalyticsDatasets/blob/main/real_estate.csv Tasks

### Data Preparation (5 marks)

1. Load the dataset on Colab

2. Display the attributes' name and their data type

3. Delete the columns num and transaction_date

4. Use house_price_per_unit as the target value and the rest of the data frame as features

5. Divide your dataset into 80% for training and 20% for test

6. Scale the columns using min-max scalers

7. Print the shape of the train and test set

NN implementation (10 Marks)

1. Implement your NN method. To predict each point (query point) of the test set, you need to:

a. Find the training point with the smallest Manhattan distance with the query point

a. Use as a prediction the target value of the point with the smallest distance to the query point

2. Compute the mean absolute error (MAE) and the mean squared error (MSE) between the test labels and the predicted values

k-NN implementation (10 Marks)

1. Extend the previous implementation by using the average of the k closest neighbours as a prediction

2. Implement the Euclidian distance as well

3. Test your approach for k values = [1, 3, 5, 7] and the two distance measures

a. Which is the best combination of k and distance?

**Reminder: You can not use any library, with the exception of pandas and NumPy. So scikit-learn is forbidden!**

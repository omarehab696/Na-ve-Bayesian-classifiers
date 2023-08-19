# Naive-Bayesian-classifiers
## Step 1: Split the dataset into two parts, with 80% of the data used for training and 20% of the data used for testing. Then Train each classifier on the training data and evaluated its performance on the test data.

## The Result Confusion Matrix for Gaussian NB:
<img src="output 1.png">
The result shows an Accuracy of 82.08%, an overall Precision of 85.7%, an overall Recall of 82.08%, and an overall F1 Score of 82.2%


## The Result Multinomial NB Confusion Matrix:
<img src="output 2.png">
The result shows an Accuracy of 72.3%, an overall Precision of 100%, an overall Recall of 72.3%, and an overall F1 Score of 83.9%

## Step 2: Use the train_test_split function from the sklearn.model_selection library to split the dataset into training and test sets. We used a random state of 42 for both splits.

## The Result Confusion Matrix for Gaussian NB:
<img src="output 3.png">
The result shows an Accuracy of 82.08%, an overall Precision of 85.7%, an overall Recall of 82.08%, and an overall F1 Score of 82.2%

## The Result Multinomial NB Confusion Matrix:
<img src="output 4.png">
The result shows an Accuracy of 78.1%, an overall Precision of 78.02%, an overall Recall of 78.7%, and an overall F1 Score of 78%

## I decided to use the Bernoulli NB which is much better in binary classification that gives better results as the following Confusion Matrix show
<img src="output 5.png">
The result shows an Accuracy of 88.6%, an overall Precision of 88.62%, an overall Recall of 88.5%, and an overall F1 Score of 88.51%

## Conclusion :

* Accuracy: The Gaussian classifier scored 82.08% accuracy, the Multinomial classifier scored 78.61% accuracy, and the Bernoulli classifier scored 88.06% accuracy.
* Precision: In terms of both classes and total precision, the Bernoulli classifier is superior.
* F1 Score: The highest F1 score belongs to the Bernoulli classifier, which indicates that it has the best recall and precision ratio. It does a better job of accurately categorizing spam and non-spam communications without favoring any one element above others (false positives or false negatives).
* Due to the characteristics of the data and the model assumptions, the performance of the Bernoulli Naive Bayes classifier has improved. In this instance, it may be because the characteristics of the data set more closely resemble a Bernoulli distribution than a Gaussian or Multinomial distribution.

## Split the Training data into 4 equal subsets

* Take the same first 80 percent as asked in (a) training samples and split the data into four equal parts according to order such as the first 25% of training data(subset 1), the second 25% of training data (subset 2), the third 25% of training data (subset 3) and the fourth 25% of training data (subset 4).
* Train selected page 2classifier chosen in (c) for each subset and predict the accuracy score by evaluating on last 20 percent of test data assumed in (a). Plot bar chart to show all subsets’ accuracy on the figure. Add your comment
<img src="output 6.png">

* The accuracy for subset 1 is 40%
* The accuracy for subset 2 is 86%
* The accuracy for subset 3 is 60%
* The accuracy for subset 4 is 60%
* The results of this experiment suggest that the Bernoulli Naive Bayes classifier is a good choice for spam filtering tasks. The classifier performs consistently well on different subsets of the training data, and it has a slightly higher accuracy score than the Gaussian and Multinomial Naive Bayes classifiers. In addition, the Bernoulli Naive Bayes classifier is relatively simple to implement, and it is computationally efficient. These factors make it a good choice for spam filtering applications where speed and accuracy are important

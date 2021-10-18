Simply calculating how many predictions were correct is sometimes misleading or too simplistic for us to understand the kinds of errors it will make in the real world. To get more detailed information, we can tabulate the results in a structure called a confusion matrix, like this:

A confusion matrix showing 2 true-negatives, 2 true-positives, 1 false-negative, and 1-false positive

The confusion matrix shows the total number of cases where:

The model predicted 0 and the actual label is 0 (true negatives; top left)
The model predicted 1 and the actual label is 1 (true positives; bottom right)
The model predicted 0 and the actual label is 1 (false negatives; bottom left)
The model predicted 1 and the actual label is 0 (false positives; top right)
The cells in the confusion matrix are often shaded so that higher values have a deeper shade. This makes it easier to see a strong diagonal trend from top-left to bottom-right, highlighting the cells where the predicted value and actual value are the same.

From these core values, you can calculate a range of other metrics that can help you evaluate the performance of the model. For example:

Accuracy: (TP+TN)/(TP+TN+FP+FN) - out all of the predictions, how many were correct?
Recall: TP/(TP+FN) - of all the cases that are positive, how many did the model identify?
Precision: TP/(TP+FP) - of all the cases that the model predicted to be positive, how many actually are positive?
# Predicting Car Acceptability
In this R notebook, I use a random forest model on a data set to predict whether a car is considered acceptable. 

The model accurately predicted 241 unacceptable cars and 93 acceptable cars. It did not identify any false positive cars and identified 12 false negatives cars

According to the accuracy score, this model scored 96.53% overall accuracy when prediciting the acceptability of a car. This measurement factors true/false positives and negatives

The model's precision score is 95.26% which means that of all the acceptable cars, this model predicted a small number of false negatives that should have been labeled at true positives when considering the acceptability of a car. 

In regards to the recall score, this model scored perfect for predicting acceptable cars in comparison to the total acceptable cars (100%). This means that the model did not predict a single false positive car. 

The Out of Bag Error Rate of the decision tree model is calculated by considering the misclassified cars in relation to the total observations. In this model, there was 3 cars that was classified as acceptable when it was actually unacceptable, and 14 cars classified as unacceptable when they were actually acceptable. The OOB score for this model is the amount of misclassified cars divided by the total observations (14+3) / (14+3+943+422) = 1.23%

The model accurately predicted 247 unacceptable cars and 93 acceptable cars. It did not identify any false positive cars and identified 12 false negatives cars

According to the accuracy score, this model scored 98.527% overall accuracy when prediciting the acceptability of a car. This measurement factors true/false positives and negatives.

The model's precision score is 93.94% which means that of all the acceptable cars, this model predicted a small number of false negatives (6) that should have been labeled at true positives when considering the acceptability of a car. 

In regards to the recall score, this model also scored perfect for predicting acceptable cars in comparison to the total acceptable cars (100%). This means that the model did not predict a single false positive car. 

The Mean Decrease Accuracy plot identifites how much accuracy the model loses when by excluding each variable. The Mean Decrease Gini is a measure of how each variable contributes to each node. The most important variables in this approach are safety_rating, num_persons, and purchase_price according to the both of these plots. 


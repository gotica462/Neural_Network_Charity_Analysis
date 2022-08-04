# Neural_Network_Charity_Analysis

## Overview of the Analysis

Use machine learning and neural networks and the features in the provided dataset to help create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup. From Alphabet Soup’s business team, we received a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. Within this dataset are a number of columns that capture metadata about each organization. We'll clean the data and provide a model to determine the probability that the money goes to a succesful charity.


## Results

### Data Procesing 

### What variable(s) are considered the target(s) for your model?

In this model we considered the target the "IS_SUCCESSFUL" column.

![image](https://github.com/gotica462/Neural_Network_Charity_Analysis/blob/main/Target%20Variable.png)

### What variable(s) are considered to be the features for your model?

Those variables include all columns, except target variable. They are as follows: EIN, NAME, APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT.

### What variable(s) are neither targets nor features, and should be removed from the input data?

Our variables that are netiher target nor features and decided to remove from the input data are the EIN and NAME columns.

![image](https://github.com/gotica462/Neural_Network_Charity_Analysis/blob/main/dropped%20columns.png)

### Compiling, Training, and Evaluating the Model?

### How many neurons, layers, and activation functions did you select for your neural network model, and why?

I used three hidden neuron layers. The first one using 120, the second one using 60 and the third using 30. I used relu activation function for best accuracy, and I used the "Tanh" method as the output layer. 

![image](https://github.com/gotica462/Neural_Network_Charity_Analysis/blob/main/neural%20model.png)

### Were you able to achieve the target model performance?

No. The original model performance target of 75% was not achieved. Our accuracy report was only 72%.

![image](https://github.com/gotica462/Neural_Network_Charity_Analysis/blob/main/results.png)

### What steps did you take to try and increase model performance?

I added a third hidden layer, change the output layer to the "Tanh", added more neurons to the hidden layers and increased the numbers of epochs. 

## Summary

The model did not reach its target accuracy at 75%, and the attemps of optimization were also a failure. We could only increased the accuracy of the model by a minimal percent, not enough to recommend it's usage. We can always try using another model as our output layer, since I don't think increasing the neurons will improve our model. Maybe we could analyse the other valuables to decrease the ammount of unique values.




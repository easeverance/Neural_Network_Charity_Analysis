# Neural_Network_Charity_Analysis

## Overview
Alphabet Soup is looking to create a machine learning and neural network that will be capable of predicting whether applicants will be successful if funded by the company. 
The team was provided with a CSV of over 34,000 organizations that have received funding from Alphabet Soup in the past years.  This data was prepocessed and loaded into a neural network where it was trained and evaluated. 

## Results

### Data Preprocessing

* The target variables in this model is: Whether the investment was successful and funds used effectively
* Features for the model were: application type and classification
* Columns - EIN and Name were remvoed as they proved to not be useful in this model

### Compiling, Training and Evaluationg the Model

* The original model contained 40 neruons, 2 hidden layers, and activation of relu.  The output layer had an activation of sigmoid.  This was used to get a base model initated to work off of for any needed improvements. 
* The original model accuracy rate was 72%.  This is below the suggested target accuracy rate of 75%
* Several steps were taken to try to optimize the model and achieve the target performance of 75%
  *     A third hidden layer was added
  *     Neurons were changed to a total of 140
  *     Epochs were changed from 100 to 500
  *     Additional binning of Income_Amt
 Target accuracy of 75% was still not achieved.  However, accuracy did go to 73%

![Optimized Accuracy](https://user-images.githubusercontent.com/90973718/151733434-e3ce0543-6bb4-495c-97fc-9fde7911f268.png)

  ### Summary
  
Trying to optimize the model did not significantly change the accuracy of the model.  Therefore, it can be concluded that adding the third hidden layer was redundant.  The data was encapsulated with just two hidden layers.  Adding any additional layers will only result in the possibility of overfitting the data.  Due to this the SVM model could possibly be a better fit. SVM's are less prone to overfitting because they are only trying to maximize distance between groups of binary classification.  




# Neural_Network_Charity_Analysis

## Overview of the analysis
The purpose of the analysis is to utilize machine learning and neural networks to create a binary classifier that is capable of predicting whether charity applicants will be successful if funded by Alphabet Soup.

## Results

### Data Preprocessing
* What variable(s) are considered to be the features for your model?
The application type, affiliation, classification, use case, organization, status, income amount, special considerations, and ask amount were the input features to the model.

* What variable(s) are considered the target(s) for your model?
The output or target was the "Is_Successful" column which results in a Yes (1) or No (0) classification.

![Charity_Columns](https://user-images.githubusercontent.com/69759624/105562644-a2e0c000-5ce0-11eb-85ae-87dd71a7d805.PNG)

* What variable(s) are neither targets nor features, and should be removed from the input data?
The non-beneficial ID columns, 'EIN' and 'NAME', were dropped from the input data because the information will not help the classifier predict if an applicant will be successful.
![Unnecessary_Columns](https://user-images.githubusercontent.com/69759624/105562642-a1af9300-5ce0-11eb-9752-d151e96a5def.PNG)

### Compiling, Training, and Evaluating the Model
* How many neurons, layers, and activation functions did you select for your neural network model?
There were 80 neurons in the first hidden layer and 30 neurons in the second hidden layer. The activation function for the first and second hidden layers was "relu". The activation function for the output layer was "sigmoid". 
![Model_Parameters](https://user-images.githubusercontent.com/69759624/105563148-a7a67380-5ce2-11eb-9808-efcd9e170f3a.PNG)

* Were you able to achieve the target model performance?
The accuracy for the model was 72.61% and did not reach the desired accuracy of 75%.

* What steps did you take to try and increase model performance?
Three attempts were taken to raise the accuracy to at least 75%.
#### Attempt #1: The column "ASK_AMT" was dropped because the values were noisy. The number of neurons in the first hidden layer was raised to 100 from 80.  Thirdly, a third hidden layer was added with 15 neurons. The accuracy was 72.58%.
![Module_19_Attempt_1](https://user-images.githubusercontent.com/69759624/105566212-8a78a180-5cf0-11eb-8be5-c771952a2b13.PNG)

#### Attempt #2: The activation function of the first hidden layer was changed to "tanh".  The accuracy was 72.62%.
![Module_19_Attempt_2](https://user-images.githubusercontent.com/69759624/105566210-89e00b00-5cf0-11eb-864a-98869bc29bcb.PNG)

#### Attempt #3: The number of neurons in the third layer was raised to 50 from 15. The The accuracy was 72.45%.
![Module_19_Attempt_3](https://user-images.githubusercontent.com/69759624/105566213-8a78a180-5cf0-11eb-8a5e-19acfef4b24b.PNG)

## Summary
* The accuracy stayed in the 72% range for the original attempt and the subsequent three attempts.

* Include a recommendation for how a different model could solve this classification problem.
Due to an accuracy less than 75% for the neural network, the recommendation is to create a binary classifier using a Support Vector Machine (SVM). The dataset is well-suited as a straightforward binary classification and the SVM may outperform the neural network.

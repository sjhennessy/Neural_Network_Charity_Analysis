# Neural_Network_Charity_Analysis

## Overview of the analysis
The purpose of the analysis is to utilize machine learning and neural networks to create a binary classifier that is capable of predicting whether charity applicants will be successful if funded by Alphabet Soup.

## Results

### Data Preprocessing
* What variable(s) are considered to be the features for your model?
The application type, affiliation, classification, use case, organization, status, income amount, special considerations, and ask amount were the input features to the model.

* What variable(s) are considered the target(s) for your model?
The output or target is the "Is_Successful" column which results in a Yes (1) or No (0) classification.

![Charity_Columns](https://user-images.githubusercontent.com/69759624/105562644-a2e0c000-5ce0-11eb-85ae-87dd71a7d805.PNG)

* What variable(s) are neither targets nor features, and should be removed from the input data?
The non-beneficial ID columns, 'EIN' and 'NAME', were dropped from the input data because the information will not help the classifier predict if an applicant will be successful.
![Unnecessary_Columns](https://user-images.githubusercontent.com/69759624/105562642-a1af9300-5ce0-11eb-9752-d151e96a5def.PNG)

### Compiling, Training, and Evaluating the Model
* How many neurons, layers, and activation functions did you select for your neural network model, and why?
* Were you able to achieve the target model performance?
* What steps did you take to try and increase model performance?

## Summary: 
Summarize the overall results of the deep learning model. 
Include a recommendation for how a different model could solve this classification problem, and explain your recommendation.

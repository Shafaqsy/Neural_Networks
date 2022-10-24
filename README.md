# Neural_Networks
## Purpose
The purpose of this analysis is to help Beks create a binary classifier With the knowledge of machine learning and neural networks that is capable of predicting whether applicants will be successful if funded by Alphabet Soup.
From Alphabet Soup’s business team, Beks received a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. Within this dataset are a number of columns that capture metadata about each organization, such as the following:

EIN and NAME—Identification columns
APPLICATION_TYPE—Alphabet Soup application type
AFFILIATION—Affiliated sector of industry
CLASSIFICATION—Government organization classification
USE_CASE—Use case for funding
ORGANIZATION—Organization type
STATUS—Active status
INCOME_AMT—Income classification
SPECIAL_CONSIDERATIONS—Special consideration for application
ASK_AMT—Funding amount requested
IS_SUCCESSFUL—Was the money used effectively

## Results
### Target Variable

The IS_SUCCESSFUL column is target variable in the model.

<img width="627" alt="img1" src="https://user-images.githubusercontent.com/107155888/197437933-3f5dc562-6502-48a5-9a71-b0101a325425.png">

### Feature Variable

The APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, INCOME_AMT, SPECIAL_CONSIDERATIONS and ASK_AMT columns are considered to be the features of the model.


### Neither Target Nor Features

The EIN, STATUS and NAME columns are neither targets nor features and should be removed from the input data.

#### How many neurons, layers, and activation functions did you select for your neural network model, and why?

I choose 80 neurons with a relu function for my first layer, 30 nuerons with a relu function for the second, and a sigmoid function for the outer layer.

<img width="562" alt="img2" src="https://user-images.githubusercontent.com/107155888/197438070-7f0b55fa-ac98-458e-92e0-48ad3aa96b2c.png">


#### Were you able to achieve the target model performance?
No, The accuracy score should be atleast more than 75%.

<img width="527" alt="img3" src="https://user-images.githubusercontent.com/107155888/197438094-40b8840c-21b7-4c09-a071-ff7087180b37.png">


#### What steps did you take to try and increase model performance?

First, I added number of neuron in each layer.

second, I used a different activation function for each hidden layer.

Third, I added another hidden layer

I have done three attempts at optimizing the model but my model does not achieve target performance. All three of them has given an accuracy score 73%.

<img width="551" alt="img4" src="https://user-images.githubusercontent.com/107155888/197438114-22a5fff4-0e4f-47b4-95e2-2de76349b953.png">
<img width="546" alt="img5" src="https://user-images.githubusercontent.com/107155888/197438118-195e3eeb-cd14-43bc-a45f-7f9a4b401fe6.png">
<img width="546" alt="img6" src="https://user-images.githubusercontent.com/107155888/197438127-9a3ad4dd-c940-4963-9315-74b8c3e428cc.png">


## Summary
Overall, the accuracy score is 73% for all three attempts at optimizing the model. I have tried droping the another feature column and I have increased the number of values for each bin in APPLICATION_TYPE coulmn. Also, I have added number of neuron, hidden layer and changed the activation function. None of these changes had increased the accuracy score.

#### RECOMMENDATION

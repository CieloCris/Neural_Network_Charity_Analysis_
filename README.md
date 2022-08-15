# Neural Network Charity Analysis


## Overview

In this challenge, the Foundation Alphabet Soup wants to predict where to make investments and charity by using a deep learning neural network model. The fictional company wants to know which applicants will be successful (or not) if they receive donations. 

The purpose of this analysis was to create a binary classifier utilizing a neural network model and tools such as Python, Pandas, and Tensorflow.


## Results


_Data Preprocessing_

- **What variable(s) are considered the target(s) for your model?** 

The "IS SUCCESSFUL" column is our target or our dependent variable.

- **What variable(s) are considered to be the features for your model?** 

The features are all the other variables that are being used in our model, such as APPLICATION_TYPE, CLASSIFICATION,  AFFILIATION, USE_CASE, ORGANIZATION, ASK_AMT, SPECIAL_CONSIDERATION, INCOME_ATM, STATUS (indepent variables). 

- **What variable(s) are neither targets nor features, and should be removed from the input data?** 

In the first attempt, we dropped the identification columns "EIN" and "NAME".  It's important to notice that in the second attempt, when we tried to optimize the model, We only removed the "EIN" column.

_Compiling, Training, and Evaluating the Model_

- **How many neurons, layers, and activation functions did you select for your neural network model, and why?**

The following screenshot shows the hidden layers, neurons, and activation functions that we choose for our first model:

![Alt text](/Resources/1.png "imagen1")

As we can see below, we optimized our model (AlphabetSoupCharity_optimized) by modifying and creating new layers, neurons, and activation functions.

![Alt text](/Resources/2.png "imagen2")

- **Were you able to achieve the target model performance?**

#### Model

![Alt text](/Resources/3.png "imagen3")

As we can see above, the performance of 75% accuracy was not achieved in our first attempt.

#### Optimized model

![Alt text](/Resources/4.png "imagen4")

In our second attempt, our model accomplished the performance of 75% accuracy (79%)

- **What steps did you take to try and increase model performance?**

We increased our model performance by including the "NAME" column in the model and adding a third hidden layer with ten neurons. We also made some adjustments and changes to our activation functions. Fortunately, the performance increased from 72% to 79%.
 
## Summary

We managed to improve our deep learning model, but it was hard to know what to change or how many layers and neurons we needed to add. We fulfill our goal by including another variable from the dataset (the "NAME" column) and adding a third hidden layer. However, we can use other classification models to achieve our purpose, such as  Random Forest Classifier or Logistic Regression. 

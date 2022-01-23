

### Neural Network Model Report

For this part of the Challenge, you’ll write a report on the performance of the deep learning model you created for AlphabetSoup.

The report should contain the following:

1. **Overview** of the analysis: Explain the purpose of this analysis.
This analysis focuses on developing a binary classifier neural network in order to predict whether the applicants for funding will be successful

2. **Results**: Using bulleted lists and images to support your answers, address the following questions.

  * Data Preprocessing
    * What variable(s) are considered the target(s) for your model?
    the column: IS_SUCCESSFUL
    * What variable(s) are considered to be the features for your model?
    APPLICATION_TYPE—Alphabet Soup application type
    AFFILIATION—Affiliated sector of industry
    CLASSIFICATION—Government organization classification
    USE_CASE—Use case for funding
    ORGANIZATION—Organization type
    STATUS—Active status
    INCOME_AMT—Income classification
    SPECIAL_CONSIDERATIONS—Special consideration for application
    ASK_AMT—Funding amount requested
    * What variable(s) are neither targets nor features, and should be removed from the input data?
    EIN, NAME
  * Compiling, Training, and Evaluating the Model
    * How many neurons, layers, and activation functions did you select for your neural network model, and why?
    The best result was my 2nd attempt, which came with 3 layers that excluded EIN, NAME, SPECIAL_CONSIDERATION_N, AND SPECIAL_CONSIDERATION_Y. Its 2nd layer had 1/2 of input layer and 3rd layer had just 1. The input layers used relu function and the output layer used sigmoid.
    * Were you able to achieve the target model performance?
    No
    * What steps did you take to try and increase model performance?
    I tried to reduce some of the features such as removing 'SPECIAL_CONSIDERATION_N' AND 'SPECIAL CONSIDERATION_Y'. I also tried change the number of layers in each layer.

3. **Summary**: Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and explain your recommendation.
    I have tried to reduce the features and adjust the numbers of layers to optimize the model. However, I wasn't able to make the score above 75%. At this point I believe using keras tuner to create nn model would be a better idea.
- - -

## Rubric

[Unit 21 - Deep Learning Homework Rubric - Charity Funding Predictor](https://docs.google.com/document/d/1SLOROX0lqZwa1ms-iRbHMQr1QSsMT2k0boO9YpFBnHA/edit?usp=sharing)

___
© 2021  Trilogy Education Services, a 2U, Inc. brand. All Rights Reserved.	

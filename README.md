### Deep-learning-challenge 
## by Olga Petrova

The nonprofit foundation Alphabet Soup wants a tool that can help it select the applicants for funding with the best chance of success in their ventures. 

This model can predict whether applicants will be successful if funded by Alphabet Soup.

## Data used: CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years.

## Data Preprocessing

- Target for the model: column IS_SUCCESSFUL, variables varied: NAME, APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT
- Features for different models:
- - features for the first model were APPLICATION_TYPE	AFFILIATION	CLASSIFICATION	USE_CASE	ORGANIZATION	STATUS	INCOME_AMT	SPECIAL_CONSIDERATIONS	ASK_AMT
- - features for the second model were columns APPLICATION_TYPE	CLASSIFICATION	USE_CASE	INCOME_AMT	SPECIAL_CONSIDERATIONS	ASK_AMT
- - features for the third model were NAME	APPLICATION_TYPE	AFFILIATION	CLASSIFICATION	USE_CASE	ORGANIZATION	STATUS	INCOME_AMT	SPECIAL_CONSIDERATIONS	ASK_AMT

## Model 1 resulted in 72% Accuracy and 0.56 Loss
## Model 2 resulted in 62.6% Accuracy and 0.63 Loss
## Model 3 resullted in 75% Accuracy and 0.51 Loss
## Started modifications on Model 3: Added layers and neurons, scaled Name column, scaled CLASSIFICATION column. This resulted in Accuracy 78.8%. Loss 0.47


How many neurons, layers, and activation functions did you select for your neural network model, and why?
Were you able to achieve the target model performance?
What steps did you take in your attempts to increase model performance?
, 


Write a Report on the Neural Network Model (30 points)
Write an analysis that includes a title and multiple sections, labeled with headers and subheaders (4 points)
Format images in the report so that they display correction (2)
Explain the purpose of the analysis (4)
Answer all 6 questions in the results section (10)
Summarize the overall results of your model (4)
Describe how you could use a different model to solve the same problem, and explain why you would use that model (6)

For this part of the assignment, you’ll write a report on the performance of the deep learning model you created for Alphabet Soup.

The report should contain the following:

Overview of the analysis: Explain the purpose of this analysis.

Results: Using bulleted lists and images to support your answers, address the following questions:

Data Preprocessing

What variable(s) are the target(s) for your model?
What variable(s) are the features for your model?
What variable(s) should be removed from the input data because they are neither targets nor features?
Compiling, Training, and Evaluating the Model

How many neurons, layers, and activation functions did you select for your neural network model, and why?
Were you able to achieve the target model performance?
What steps did you take in your attempts to increase model performance?
Summary: Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and then explain your recommendation.
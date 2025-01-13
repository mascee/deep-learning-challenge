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

## Model 1 used 6 neurons on the fisrt layer, 6 on the second layer, and 1 for the output. Model 1 resulted in 72% Accuracy and 0.56 Loss
## Model 2 used 6 neurons on the fisrt layer, 6 on the second layer, and 1 for the output. resulted in 62.6% Accuracy and 0.63 Loss
## Model 3 used the same number of neurons as previous ones. Resullted in 75% Accuracy and 0.51 Loss
## Started modifications on Model 3: scaled Name column, scaled CLASSIFICATION column. 3 layers, 80+30 neurons, plus 1 output neuron. 75% Accuracy and 0.51 Loss
## Model 4: scaled Name column differently, scaled CLASSIFICATION column differently. 3 layers, 80+30 neurons, plus 1 output neuron. This resulted in Accuracy 78.8%. Loss 0.47
## Model 5: Transformed INCOME_AMT column to Integer, as it contained dashes and letters 'M'. Performed additional model #5 on it. It did not iprove my best result, stayed at around 78%.
## I used many other models, but deleted them, as they performed around 74-75% accuracy and I thought it was redundant. Changing number of neurons, and layers did not improve Accuracy much, but putting values of several columns into different buckets helped with accuracy.
## I am not completely satisfied with the performance, but this is the best result I have. 


### Overall I have around 79 accruracy for prediction if the no-profit ask will be successfull.

### Recomendation. Columns 'NAME', 'CLASSIFICATION',  'AFFILIATION', 'INCOME_AMT<=': Data is scewed to "Other" bucket. If changing cutoff, the result is too many buckets. May need to work in that direction to improve performance.

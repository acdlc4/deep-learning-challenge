# deep-learning-challenge 
---
# Overview

#### A hypothetical, nonprofit foundation (Alphabet Soup) has commissioned a tool that can help it select the applicants for funding with the best chance of success in their ventures. Using machine learning and neural networks, the use of the features in the provided dataset will be pertinent to create a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup.
---
# Results

### Data Preprocessing
What variable is the target for your model?
- The target selected for this model is the "IS_SUCCESSFUL" column as it provides the result of whether or not the investment in a particular venture was used productively.

What variables are the features for your model?
- The features of this model consist of the following fields:
  - NAME - Identification column
  - APPLICATION_TYPE - Alphabet Soup application type
  - AFFILIATION - Affiliated sector of industry
  - CLASSIFICATION - Government organization classification
  - USE_CASE - Use case for funding
  - ORGANIZATION - Organization type
  - INCOME_AMT - Income classification
  - SPECIAL_CONSIDERATIONS - Special consideration for application
  - STATUS - Active status
  - ASK_AMT - Funding amount requested

What variable was removed from the input data because it is neither a target nor a feature?
- The variable removed was EIN (Employer Identification Number) due to the fact that the system could misconstrue this data as a measure of value as opposed to a unique identifier of an organization.


###Compiling, Training, and Evaluating the Model
How many neurons, layers, and activation functions did you select for your neural network model, and why?
- This model was created with 1) an additional hidden layer (to a total of three), each with 2) modifications to the levels of neurons as this helped to increase the model's accuracy above the needed efficacy level of 75%.  Third modification involved 3) changing the second and third output functions to 'sigmoid' from 'relu', which also helped to increase accuracy results. Epoch numbers were held constant as compared to the original model at 100.

Were you able to achieve the target model performance?
- Target model performance was achieved at 78.11%, which is above the 75% threshold.

What steps did you take in your attempts to increase model performance?
- As compared to the original model, the replacing of the CLASSIFICATION field for the NAME field and the addition of another hidden layer helped significantly increase overall model performance.
---
# Summary
- By successfully modifying the original model, the accuracy of the performance of the model was refined to be able to classify successful results over 75% of the time on average.

- Based on the last five model results, an applicant has over an 80% chance of success if the following criteria are met:
  - APPLICATION_TYPE is from the following list: [T3 to T8, T10, T19]
  - Applicants have applied 10 or more times

- An alternative model to recommend is the Histogram-based Gradient Boosting Classifier estimator which was designed for classification tasks.  As seen with the example below, the accuracy result provides a result of over the required 75%, at 76.8%.

##
### File locations
#### Jupyter notebooks:
- https://github.com/acdlc4/deep-learning-challenge/blob/main/AlphabetSoupCharity.ipynb
- https://github.com/acdlc4/deep-learning-challenge/blob/main/AlphabetSoupCharity_Optimization.ipynb
#### HDF5 results:
- https://github.com/acdlc4/deep-learning-challenge/blob/main/AlphabetSoupCharity.h5
- https://github.com/acdlc4/deep-learning-challenge/blob/main/AlphabetSoupCharity_Optimization.h5

#### Report on the User-Designed Neural Network Model is located at end of AlphabetSoupCharity_Optimization.ipynb notebook link provided above

#### CSV data resource:
- https://static.bc-edx.com/data/dl-1-2/m21/lms/starter/charity_data.csv
--- 
### Any questions?

Feel free to send a message to acdlc4@gmail.com with any questions / comments. Inspiration and credit for any code used is from work done during my attendance in the 2024 Northwestern University Data Analysis Bootcamp class sessions.



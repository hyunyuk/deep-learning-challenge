# deep-learning-challenge
Module 21 Challenge

# Overview of the Analysis
Module 21 was about the nonprofit foundation Alphabet Soup wanting a model to help select applicants that has a better chance for success in their ventures. Therefore, using machine learning, we will create a binary classifier that can predict which applications will be sucessful if chosen. 

# Results

## Data Preprocessing
- Removed "EIN" and "NAME" from the model, which the remaining columns were used as our features
- "IS_SUCCESSFUL" was the target variable, using 0 as no and 1 as yes
- "APPLICATION_TYPE" and "CLASSIFICATION" were replaced with "Other" due to cutoff
- Converted the data to numeric to get a better idea of the data

## Compiling, Training, and Evaluating the Model

### Neural Network
- Contained three layers
- Generated a total of 6461 parameters
- Accuracy was roughly 73% which is slightly less than the desired 75%

### Optimization Neural Network
- The only change in the second attempt was adding "NAME" back in the dataset.
- Contained three layers
- Generated a total of 38701 parameters
- Accuracy was roughly 79% which is over the desired 75%

# Summary
The neural network was very close in achieving sucess, falling just 2% short of our desire accuracy. On the second attempt, after adding back the feature "NAME" into the model results in a significant improvement, yielding a better accuracy with 79% which exceeded our desired percentage of 75%. Although we only added "NAME", we did take out applicants that had less than 5 occurence. In the end, the model gave a better prediction on whether a specific applicant will be successful with Alphabet Soup. 
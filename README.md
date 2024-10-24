# deep-learning-challenge
Module 21 Challenge - Deep Learning

PURPOSE OF EVALUATION:
The purpose of this analysis is to predict whether or not applicants who are seeking funding will be successful or not. This analysis reviews more than 34,000 organizations that have received funding from Alphabet Soup over the years, allowing us to see whether or not the funds were used effectively. 

DATA PREPROCESSING:
- The target for this model is to reach the "IS_SUCCESSFUL" column, which shoes that the money was used effectively.
- Variables that are considered features for this model include: NAME, APPLICATION, TYPE, AFFILICATION, CLASSIFICATION, USE_CASE, INCOME_AMT, SPECIAL_CONSIDERATIONS, STATUS, ASK_AMT.
- Variables that could be removed from the dataset because they are neither targets nor features are "EIN", "SPECIAL_CONSIDERATIONS", and STATUS (which has the value of 1 for all rows). 

COMPILING, TRAINING AND EVALUATING THE MODEL
1. For this analysis, there are three hidden layers, all with many neurons, which increased the accuracy to above our goal of 75%. Changes made throughout the analysis included changing the activation function from 'relu' to 'sigmoid', which increased the accuracy. The number of epochs was not increased or decreased. 
2. The target measure of success was reached with our analysis coming in at just over 77%.
3. The most effective steps taken to increase accuracy was in changing the activation function to 'sigmoid' for the 2nd and 3rd layers. Converting columns (such as the NAME column) into data points also had a significant effect on the accuracy.

SUMMARY:
In summary, increasing the accuracy allowed us to correctly classify the test data 77% of the time. We learned that an applicant has an over 75% change of being successful if they have multiple applications, with the applications being one of the following: T3, T4, T5, T6, T7, T10, T19). Additionally, the application needs to have the following classification: C1000, C2000, C3000, C1200, C2100.
Lastly, we found that the best model for this type of analysis is the Random Forest model because it is effective for classification. The Random Forest model produced almost 78% accuracy. 

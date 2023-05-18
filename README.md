# credit-risk-classification
Module 20 - Supervised Learning 

## OVERVIEW ##
    This Analysis helps banks find the right prediction model to use (that gives the optimum result), in order to make decisions in lending  out loans to borrowers.
    Variables were extracted from lending_data.csv file.  These were then trained & tested using Balanced Accuracy score, Confusion Matrix, and Classification report.

## THE RESULTS ##

 # Logistic Regression Model with Original Data #
    * Balanced Accuracy Score: 0.9442676901753825 This tells us the overall accuracy score of the model. 
    * Precision Score: 
        -healthy loan (0): 1.00 This tells us how close the numbers for healthy loan are clustered in the model
        -high-risk loan (1): 0.87 This tells us that the high-risk loan data in the model is slightly scattered, but is distinct (at 87% precision)
    * Recall Score: 
        -healthy loan (0): 1.00 Healthy loans data are 100% correctly identified in the model 
        -high-rsik loan (1): 0.89 high-risk loan predictions are 89% correctly identified

# Logistic Regression Model with Resampled Training Data #
    * Balanced Accuracy Score:  0.9945026387334079 This tells us the overall accuracy score of the model is close to 100%  
    * Precision Score: 
        -healthy loan (0): 0.99 This tells us how close the numbers for healthy loan are clustered in the model
        -high-risk loan (1): 0.99 This tells us that the high-risk loan data in the model are well clustered
    * Recall Score: 
        -healthy loan (0): 0.99 Healthy loans data are 99% correctly identified in the model 
        -high-rsik loan (1): 0.99 high-risk loan predictions are 99% correctly identified


## SUMMARY ##
 There is a high accuracy of the LogisticRegression model when predicting healthy loan (0), and high-risk loan (1).  This can be illustrated through the classification reports using Original Data & Resampled Training Data in the LogisticRegression models.  Healthy loans is accurately predicted in both methods showing 99-100% accuracy.  High-risk loan prediction in both methods differ by over 10%, but overall accuracy score is at 94% using original data which indicates a good LogisticRegression prediction model. I would likely recommend using the original data in the LogisticRegression model since since it could accurately predict healthy loans, although there are a number of factors affecting high-risk loans prediction, the score is still acceptable and there's lesser risk in overfitting.
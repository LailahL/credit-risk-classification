# credit-risk-classification
Module 20 - Supervised Learning 

## OVERVIEW ##
    This Analysis helps banks find the right prediction model to use (that gives the optimum result), in order to make decisions in lending  out loans to borrowers.

## THE RESULTS ##
    * Balanced Accuracy Score: 0.9442676901753825 This tells us the overall accuracy score of the model. 
    * Precision Score: 
        -healthy loan (0): 1.00 This tells us how close the numbers for healthy loan are clustered in the model
        -high-risk loan (1): 0.87 This tells us that the high-risk loan data in the model is slightly scattered, but is distinct (at 87% precision)
    * Recall Score: 
        -healthy loan (0): 1.00 Healthy loans data are 100% correctly identified in the model 
        -high-rsik loan (1): 0.89 high-risk loan predictions are 89% correctly identified
## SUMMARY ##
 There is a high accuracy of the LogisticRegression model when predicting healthy loan (0), and high-risk loan (1).  This can be illustrated through the classification report, showing 100% for healthy loan prediction, but the prediction for high-risk loan is only 87%. Balanced accuracy score is at 94% which indicates a good overall LogisticRegression prediction model. I therefore recommend using this model since since it could accurately predict healthy loans, although there are a number of factors affecting high-risk loans prediction, the score is still over 85%, and is acceptable.
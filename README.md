# RandomForest

1. Decision Tree- A Decision Tree is a supervised machine learning algorithm used for classification and regression.
It splits data based on feature values into a tree-like structure, where the Internal nodes represent decisions based on a feature, Leaves represent the final output class or value.
A decision tree classifier is trained to classify whether a person has heart disease based on features like age, cholesterol.

2. Random Forest- A Random Forest is an ensemble method that builds many decision trees and combines their outputs to make a final decision.It reduces overfitting and improves accuracy. 
Each tree is trained on a random subset of data and features.
A forest of 100 trees is built and the final prediction is made using majority voting across trees.

3. Classfifictaion-  The model predicts the target column ("target") which is:
0: No Heart Disease  1: Heart Disease
The model uses input features like age, chol, thalach, etc., and classifies based on splitting rules created during training.

4. Visualize a Decision Tree-
class_names: Labels for the target classes.
feature_names: Names of the input features.
filled=True: Colors nodes based on class probability.
This tree helps you understand how decisions are made.
Each split represents a decision like: “Is cholesterol > 250? → go left or right depending on answer.”

5. Interpret Feature Importance-
A bar graph shows features like cp, thal, or ca with high importance.
These are the features the model relied on most across the trees in the Random Forest.
A higher value means that feature helped reduce error more during tree splits.

6. To make it unique and more insightful,I have done the calssfication report and the ploted the ROC Curve and the Confusiin Matrix. 
Confusion Matrix helps you see if model is biased toward one class.
Interpretation-
Diagonal values = correct predictions
Off-diagonal = errors

7. Classfication Report is calculating the Precision, Recall, and F1 Score.
Interpretation:
The curve shows how threshold tuning affects performance.
The higher the curve bows to the top-left, the better.
AUC > 0.9 is excellent; >0.8 is good.

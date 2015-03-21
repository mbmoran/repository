# Machine-Learning
Assignment for Coursera Class Machine Learning

This repo contains a written report as Machine_Learning_Project_v3_submit.html and 3 figures.

### TITLE: Machine Learning Course Project: March 2015
#### A Predictive Model for Evaluating the Execution of a Unilateral Dumbbell Bicepts Curl
#### With Dataset from the Paper: "Qualitative Activity Recognition of Weight Lifting Exercises"

#### I.  Executive Summary:

Using the Weight Lifting Exercises (WLE) dataset to predict whether or not a Unilateral Dumbbell Biceps Curl was performed according to an established standard(see II. for paper citation), three random forest classification models were developed and compared:  (1) 54 predictor variables, (2) 30 variables and (3) 2 variables. In conclusion, The 2-variable model accuracy and out of sample error measures were about as good as for the 54 variable model while reducing overfitting issues apparent with the latter, and the 2 variable model predicted the exercise class in the final 20 test case set 100% accurately. The 2 classification variables are: (1) num _ window and (2) row_belt, found from cross validation and GINI variable importance criterion. Extremely accurate prediction results for even a 2 variable model indicate some degree of dataset dependency (or overfitting) may still exist. If the final model was used to predict exercise classe on data derived from a new independent experiment using different subjects and sensor measurements, it may not be as robust nor the predictions as accurate.

#### II. Introduction: Data Source and Project Questions:

The Weight Lifting Exercises (WLE) dataset contains body sensor accelerometer data from six males (ages 20-28) who performed 10 repetitions of the Unilateral Dumbbell Biceps Curl in five different ways(i.e., classes): exactly according to the specification (Class A), throwing the elbows to the front (Class B), lifting the dumbbell only halfway (Class C), lowering the dumbbell only halfway (Class D) and throwing the hips to the front (Class E).

Class A corresponds to the specified execution of the exercise, while the other 4 classes correspond to common mistakes.

Paper Citation: *Velloso, E.; Bulling, A.; Gellersen, H.; Ugulino, W.; Fuks, H. Qualitative Activity Recognition of Weight Lifting Exercises. Proceedings of 4th International Conference in Cooperation with SIGCHI (Augmented Human '13) . Stuttgart, Germany: ACM SIGCHI, 2013.*

WLE Dataset documentation: http://groupware.les.inf.puc-rio.br/public/papers/2013.Velloso.QAR-WLE.pdf

**Project Goals:**

**1.  Build and crossvalidate a predictive model for evaluating the execution of a Unilateral Dumbbell Biceps Curl, using class of exercise as the predicted value. Discuss model selection process and quantify uncertainty (out of sample error).**

**2.  Use the model to predict class of exercise for a test set of 20 subjects.**

# Credit_Risk_Analysis

## Project Overview
For this project, different techniques were used to train and evaluate models with unbalanced classes. The project required the use of imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling.  The overall question is to determine a person's credit risk based off of some input or features that were received from the LendingClub.  A large dataset was retrieved and loaded to evaulate and attempt to predict credit risk.   

Deliverable 1 requirements: use the oversampling RandomOverSampler and SMOTE algorithms and then use the undersampling ClusterCentroids algorithm, Using these algorithms, resample the dataset, view the count of the target classes, train a logistic regression classifier, calculate the balanced accuracy score, generate a confusion matrix, and generate a classification report

## Results
There is a bulleted list that describes the balanced accuracy score and the precision and recall scores of all six machine learning models
Six machine learning models were created and used as part of this analysis.  Before the models were run, the data was cleaned by removing irrelevant columns and by converting strings to numerical values. The results of each model is below with details included. 

1. (Oversampling) RandomOverSampler Model- 

* Balanced Accuracy Score:  61%

![B80AF95B-BBF8-46BF-A744-19D5FF16D943_4_5005_c](https://user-images.githubusercontent.com/96222437/165003302-0f9d5eb2-c455-4d06-853a-4e43e3507dde.jpeg)


* Precision and Recall Scores: 
    High Risk - has a precision rate of 1% and recall rate of 67%. 
    Low Risk - has a precision rate of 100% and a recall rate of 54%.

![8E1F841B-E3F9-4E87-ABD5-52A6501B18BE_4_5005_c](https://user-images.githubusercontent.com/96222437/165001813-bf6193ed-6a5d-4c1d-8c94-47a696e509cc.jpeg)

![6BA57CDE-1A61-40B8-94C2-6B68FD1B2289_4_5005_c](https://user-images.githubusercontent.com/96222437/165001819-f930a7ff-776a-441f-b85b-deef9b875887.jpeg)

2. SMOTE - 

* Balanced Accuracy Score: 67%

![B96BC433-2BCC-4989-AFB0-33A63C2D8812_4_5005_c](https://user-images.githubusercontent.com/96222437/165002111-f7c78242-3ea9-4ed9-be3d-c296de398b0e.jpeg)


* Precision and Recall Scores: 
    High Risk - has a precision rate of 1% and recall rate of 64%. 
    Low Risk - has a precision rate of 100% and a recall rate of 69%.  This is improved over the first oversampling model, RandomOverSampler.
    
 ![7D78EC65-4CEB-41E0-B4CD-9AB778B1C877_4_5005_c](https://user-images.githubusercontent.com/96222437/165001977-8d2e0b96-a394-4879-99eb-7bc70c49c1ef.jpeg)

![7EF1BB95-6435-4AE2-B3AD-990E422BAA6B_4_5005_c](https://user-images.githubusercontent.com/96222437/165001980-47848a87-b400-492c-804c-5eff5e273784.jpeg)

3. (UnderSampling)ClusterCentroids - 

* Balanced Accuracy Score: 66.5%

![9F8E55E4-FB5D-452A-8FB0-334ADF7C4061_4_5005_c](https://user-images.githubusercontent.com/96222437/165002516-fb326075-5f7d-476e-b44c-956dc6a4d774.jpeg)

* Precision and Recall Scores: 
    High Risk - has a precision rate of 1% and recall rate of 69%. 
    Low Risk - has a precision rate of 100% and a recall rate 40%.

![45E9380C-22E6-46EE-B575-CDCC8E0AEF9D_4_5005_c](https://user-images.githubusercontent.com/96222437/165002478-03eab4d2-0377-4e89-ab8b-8959bf9f9957.jpeg)

![0C319788-10D5-49FD-9BF7-AF8D1123E77B_4_5005_c](https://user-images.githubusercontent.com/96222437/165002489-2e063709-7700-49e2-8541-7c2e02b5f8d8.jpeg)

4. SMOTEENN -

* Balanced Accuracy Score: 54.4%

![FD102D28-C7A2-4719-982B-737FB126B80F_4_5005_c](https://user-images.githubusercontent.com/96222437/165002655-cc67f04f-d9ea-4536-9a7d-5d8f3232150a.jpeg)

* Precision and Recall Scores: 
    High Risk - has a precision rate of 1% and recall rate of 73%. 
    Low Risk - has a precision rate of 100%% and a recall rate 60%.

![070C18C8-8ADF-4193-8361-5470F2E58AA7_4_5005_c](https://user-images.githubusercontent.com/96222437/165002664-c4b1c226-be38-4d93-ba58-b61fb79784f9.jpeg)

![97270F52-222A-449F-B78A-BA4EA85CDDA9_4_5005_c](https://user-images.githubusercontent.com/96222437/165002672-e4ce90d3-6cd5-424c-8c2c-54c8e2ba28d7.jpeg)

5. (Ensemble Learner)BalancedRandomForestClassifier - 

* Balanced Accuracy Score: 78.9%

![C5C3889C-4298-4781-AEE5-F6FE498FFB6D_4_5005_c](https://user-images.githubusercontent.com/96222437/165002982-767ade7b-c035-441f-9752-4695349278d2.jpeg)


* Precision and Recall Scores: 
    High Risk - has a precision rate of 3% and recall rate of 70%. 
    Low Risk - has a precision rate of 100% and a recall rate 87%.


![0800DF16-8F58-4415-A1E3-9C1C3D0B691B_4_5005_c](https://user-images.githubusercontent.com/96222437/165003016-207c884b-6fd0-4015-9e84-a089dc557ba1.jpeg)

![55E0CFE3-C2CC-4283-86FC-95F3D68C75EE_4_5005_c](https://user-images.githubusercontent.com/96222437/165002998-80bf28e7-9314-4de7-901b-412c735c2500.jpeg)


6. EasyEnsembleClassifier - 

* Balanced Accuracy Score: 93.1%

![C5F4A0DD-EE11-4FF0-BE55-9892AEDF15D3_4_5005_c](https://user-images.githubusercontent.com/96222437/165002970-ba575736-9b38-4283-8799-2ae81937095f.jpeg)


*Precision and Recall Scores: 
    High Risk - has a precision rate of 9% and recall rate of 92%. 
    Low Risk - has a precision rate of 100% and a recall rate 94%.  

![4EBA7D1E-5473-402B-8156-F9B7B52EFEFB_4_5005_c](https://user-images.githubusercontent.com/96222437/165002960-b1a54123-6928-41f8-878c-229ef580a6b6.jpeg)

![152FE375-7962-4506-9A1C-BA3085F54EF9_4_5005_c](https://user-images.githubusercontent.com/96222437/165002956-f4e927ff-f563-4675-9930-0fff41691a2d.jpeg)


## Summary

All six models faired average or above for accuracy rating.  However the clear choice for predicting credit risk would be to use the Easy Ensemble Classifier.  That model had an accuracy score of 93%.  This model also had the highest precision rate, 9%, and the best recall or sensitivity rate of 92%.  These numbers prove that the Easy Ensemble is an accurate and dependable model for identifying high risk clients.  

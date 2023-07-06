# Network model report
Neural Network Model Report
1.	Overview
With the given information, Alphabet Soup intends to use existing or previous data on award of funding criteria going forward. A  machine learning tool is therefore ideal for this purpose. This tool will use the previous data of about 34,000 organizations that have received funding from the organization over the years. A binary classifier will developed to determine wheather an applicant is successful or not. 
2.	Data Pre-processing
-	The dataset provided has 12 columns.
-	Target variable for the data is “IS_SUCCESSFUL” column.
-	The features for the model are “APPLICATION_TYPE”, “AFFILIATION”, “CLASSIFICATION”, “USE_CASE”, “ORGANIZATION”, “STATUS”, “INCOME_AMT”, “SPECIAL_CONSIDERATIONS”, “ASK_AMT”, “IS_SUCCESSFUL”
-	Irelevant columns: the “NAME” and “EIN” columns were found not to have a statistiscal impact in the data set and hence were removed. 
-   Binning was done on "CLASSIFICATION" and "APPLICATION TYPE" columns to reduce the length of dummies and redundance

3. Results- 1st Round
-   Two (2) hidden layers and 1 output layer were used
-	The first hidden layer had 80 neurons while the second hidden layer had 30 neurons.
-	This gave an accuracy of 72.98% which was was low.

4. Results- 2nd Round
-	To increase the performance of the model the following adjustments were made
    -   Removed columns "ORGANIZATION", "STATUS" and "APPLICATION_TYPE" which I considered not to be of significant impact. 
    -   The range of binning was adjusted downwards for "CLASSIFICATION" and "APPLICATION TYPE". 
    -   The number of nurons were adjusted severally
    -   The number of layers was also adjusted upwards then downwards
    -   The output layer was adjusted to “tahn” and the “leakey RELU” functions. 
    Sigmoid function had better results. 
    The best accuracy achieved in 2nd round was 70.30%
 

3.	Summary
The results for both models were low. A further understanding is required on the impact of each variable, further iterations untill best accuracy is reached for raliability. 

# Stack Overflow Tag Predictor.

## What is Stack Overflow Tag Predictor?
Stack Overflow Tag predictor is a application in which we try to generate the suitable tags for the stack overflow query post. The application suggests tags based on the text processing of body and title of the query being posted on the forum. 

## Methodology
### Overview:
We have made use of Information Retrieval methods and text processing methods to generate precise tags which are having very high similarity score.

### Implementation:
The application has been developed following the below mentioned approach.
- Data Loading
- Data Preprocessing
- TF-IDF Vectorizer
- Model Selection and Implementation
- Model Validation.

#### Data Loading:
In this step we load the queries which are used to develop the predictor. The input file contains the queries where in which we have title and body as separate attributes. The file is read as a CSV, and we then make use of data frames for the further development process.


#### Data Preprocessing:
Initially in data preprocessing few unnecessary columns have been dropped and, have dropped rows which are having more than 90% of null values.

#### TF-IDF Vectorizer:
This step is performed to convert the textual data of the query especially body and the title data into a vector space which can be used in the model development and implementation. 

#### Model Selection and Implementation:
This application makes use of a few common model used in text prediction such as SGD-Classifier, Logistic Regression, Linear-SVC, etc. We transform the data into vector space and then fit the data with these models and then train our models.

#### Model Validation:
In this step we take a test data set and perform the similar operations as followed for training and then we make the prediction using the models which were trained on the training data. The accuracy  and similarity score are then recorded and the interesting point to note is that we are more interested in similarity score rather than accuracy as we want to know how similar are the predicted tags to the actual tags.

### Conclusion:

We were successful in predicting the tags which high similarity score. The predicted and the actual tags generated are almost very similar.


# COMP34812 Natural Language Understanding Coursework (Natural Language Inference)

## data sources or code bases used(Method A)

* pandas
* numpy
* sklearn.feature_extraction.text.TfidfVectorizer
* sklearn.linear_model.LogisticRegression
* scipy.sparse.hstack
* nltk

## About

 `Group47_TrainAndDev_A.ipynb` generates TfidfVectorizer feature matrix with train/dev data and uses train data feature matrix to create Logistic Regression model. It saves model as `NLI_A_model.pkl` and `tfidf_vectorizer_train.pkl`. It also predict and evalaute the result of train data set and validation dataset.
 `Group47_Demo_A` loads `NLI_A_model.pkl` and `tfidf_vectorizer_train.pkl` as model, pre-process `test.csv`, precidict the result of `test.csv` and save the prediction as `Group_47_A.csv`

 To run `Group47_TrainAndDev.ipynb`, path needed:
 
 path:
 * "./training_data/NLI/train.csv"
 * "./training_data/NLI/dev.csv"

 To run `Group47_TrainAndDev_A.ipynb`, file and path needed:
 
 file:
 * `NLI_A_model.pkl`
 * `tfidf_vectorizer_train.pkl`
 path:
 * "./test_data/NLI/test.csv"


## data sources or code bases used(Method B)

* pandas
* numpy
* tensorflow.keras.models
* tensorflow.keras.utils
* tensorflow.keras.preprocessing.sequence
* tensorflow.keras.preprocessing.text
* tensorflow.keras.layers
* tensorflow.keras.optimizers
* tensorflow.keras.callbacks
* matplotlib.pyplot

## About

 `Group47_TrainAndDev_B.ipynb` generates `model_weights.keras` and `predictions_validation.csv` as the output. This file using the method of BiLSTM to train the 26k hypothesis and premise pair.
 To run `Group47_TrainAndDev_B.ipynb`, path needed:
 
 path:
 * "./training_data/NLI/train.csv"
 * "./training_data/NLI/dev.csv"

 To run `Group47_TrainAndDev_B.ipynb`, file and path needed:
 
 file:
 * `model_weights.keras`
 path:
 * "./test_data/NLI/test.csv"

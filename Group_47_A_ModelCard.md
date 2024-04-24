---
{}
---
language: en
license: cc-by-4.0
tags:
- text-classification
repo: https://github.com/HaojingTONG/Group47

---

# Model Card for Yida_Zhuge-Haojing_Tong-NLI

<!-- Provide a quick summary of what the model is/does. -->

This model used Logistic Regression to train a model to predict logical relationship between premise and hypothesis


## Model Details

### Model Description

<!-- Provide a longer summary of what this model is. -->

This model used 26k premise-hypothesis pair dataset to train a logical relationship prediction model between premise and hypothesis with Logistic Regression

- **Developed by:** Yida Zhuge and Haojing Tong
- **Language(s):** English
- **Model type:** Supervised
- **Model architecture:** Logistic Regression
- **Finetuned from model [optional]:** Logistic Regression

### Model Resources

<!-- Provide links where applicable. -->

- **Repository:** [More Information Needed]
- **Paper or documentation:** https://www.researchgate.net/publication/242579096_An_Introduction_to_Logistic_Regression_Analysis_and_Reporting

## Training Details

### Training Data

<!-- This is a short stub of information on the training data that was used, and documentation related to data pre-processing or additional filtering (if applicable). -->

26k premise-hypothesis pair dataset.

### Training Procedure

<!-- This relates heavily to the Technical Specifications. Content here should link to that section when it is relevant to the training procedure. -->

#### Training Hyperparameters

<!-- This is a summary of the values of hyperparameters used in training the model. -->


      - inverse of regularization strength : 0.26

#### Speeds, Sizes, Times

<!-- This section provides information about how roughly how long it takes to train the model and the size of the resulting model. -->


      - overall training time: 5 seconds
      - model size: 1MB

## Evaluation

<!-- This section describes the evaluation protocols and provides the results. -->

### Testing Data & Metrics

#### Testing Data

<!-- This should describe any evaluation data used (e.g., the development/validation set provided). -->

3.3k premise-hypothesis pair dataset.

#### Metrics

<!-- These are the evaluation metrics being used. -->


      - Precision
      - Recall
      - F1-score
      - Accuracy

### Results

The model obtained an F1-score of 70% and an accuracy of 66%.

## Technical Specifications

### Hardware


      - RAM: at least 8 GB
      - Storage: at least 1GB

### Software


      - sklearn
      - nltk

## Bias, Risks, and Limitations

<!-- This section is meant to convey both technical and sociotechnical limitations. -->

Any inputs (concatenation of two sequences) longer than
      512 subwords will be truncated by the model. Do not suggest any input are not English

## Additional Information

<!-- Any other information that would be useful for other people to know. -->

The hyperparameters were determined by experimentation
      with different values.

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

This is a NLI training model using the method of BiLSTM to predict the relationships between hypothesis and premise.


## Model Details

### Model Description

<!-- Provide a longer summary of what this model is. -->

This model used 26k premise-hypothesis pair dataset to train a BiLSTM logical prediction model between premise and hypothesis using the method of BiLSTM method.

- **Developed by:** Yida Zhuge and Haojing Tong
- **Language(s):** English
- **Model type:** Supervised
- **Model architecture:** BiLSTM
- **Finetuned from model [optional]:** BiLSTM

### Model Resources

<!-- Provide links where applicable. -->

- **Repository:** [More Information Needed]
- **Paper or documentation:** https://d1wqtxts1xzle7.cloudfront.net/89484404/1808.08762v1-libre.pdf?1660230722=&response-content-disposition=inline%3B+filename%3DNatural_Language_Inference_with_Hierarch.pdf&Expires=1713974607&Signature=MNMSsaNN5386a1glxdZqNSsdije6IX4EGcrld2vD28Vv99Z7Q0yMV9f2FXmjaMDeL4tyiFHrezzNbsEw8ki-NsW~4Wd8T7uiHah6ooX0pv2MEqRa3W~0s2iGG6q3eWkZyveUTjMeRFzRusji6ngidzkVlzlDejglMoOf0QN7L6gc8zMnifam5So7vk3Stre5aRcqa01wel2YGG-E-KM3SiA2Q64jFCdYRd3bu9I3oPPpor7USxBUuq1updyH9dxGbYJpebWbsOpO8MRZ7j3puVwQm-l1TjPPh8dAa5SnXXrKFPL5ogsrpVXU-64MGxdwuKy1XtTmPBoVIh55WDmSrw__&Key-Pair-Id=APKAJLOHF5GGSLRBV4ZA

## Training Details

### Training Data

<!-- This is a short stub of information on the training data that was used, and documentation related to data pre-processing or additional filtering (if applicable). -->

26k premise-hypothesis pair dataset.

### Training Procedure

<!-- This relates heavily to the Technical Specifications. Content here should link to that section when it is relevant to the training procedure. -->

#### Training Hyperparameters

<!-- This is a summary of the values of hyperparameters used in training the model. -->


      - learning_rate: 0.0001
      - train_batch_size: 64
      - eval_batch_size: 64
      - num_epochs: 50

#### Speeds, Sizes, Times

<!-- This section provides information about how roughly how long it takes to train the model and the size of the resulting model. -->


      - overall training time: 8mins
      - duration per training epoch: 40 seconds
      - model size: 31.1MB

## Evaluation

<!-- This section describes the evaluation protocols and provides the results. -->

### Testing Data & Metrics

#### Testing Data

<!-- This should describe any evaluation data used (e.g., the development/validation set provided). -->

3.3k premise-hypothesis pair dataset.

#### Metrics

<!-- These are the evaluation metrics being used. -->


      - Accuracy: 68.5%

### Results

The model obtained accuracy of 68.5% at the epoch 4.

## Technical Specifications

### Hardware

[More Information Needed]

### Software


      - Tensorflow 2.16.1

## Bias, Risks, and Limitations

<!-- This section is meant to convey both technical and sociotechnical limitations. -->

N/A

## Additional Information

<!-- Any other information that would be useful for other people to know. -->

N/A

# Identification of pseudothrombocytopenia in blood smears


Final project for the Building AI course

## Summary
This project aims to detect the presence of platelet aggregates/microclots in peripheral blood smears, simplifying the differentiation between pseudothrombocytopenia and real thrombocytopenia.


## Background

Pseudothrombocytopenia consists of a false decrease in the platelet count and can be the result of EDTA (anticoagulant)-dependent platelet aggregation, microclots formed during difficult and time-consuming blood collections, cold agglutinins or even improper blood sample handling.
Due to the possible presence of platelet aggregates or microclots in the blood samples, automated platelet counting can be inaccurate, leading to potential misdiagnoses of thrombocytopenia.
An automated platelet count lower than the reference value or than a previous result from the same patient implies confirmation by microscopic observation of the blood smear, resulting in greater time consumption to obtain analytical results.
In the laboratory routine, as a biomedical scientist, this is a very commom and frequent issue, always requiring confirmation and validation by a trained and qualified professional.


## How is it used?

Several images of the selected blood smears are digitalized. 
Once the model is trained, the software extracts features from those digital images and analyses it in order to detect the presence of platelet aggregates/microclots.
When platelet aggregates/microclots are detected, the software will block the result and recommend confirming the platelet count using another method (e.g. optical method) or repeating the blood collection using a different anticoagulant (e.g. sodium citrate). Otherwise, thrombocytopenia is confirmed and the result is automatically validated.


<img src="https://github.com/user-attachments/assets/07ecbc90-edc4-4b63-85d6-a04bf155af53" width="600">

<img src="https://github.com/user-attachments/assets/bdea7f8f-768f-4fdb-abe7-69628b130086" width="600">




## Data sources and AI methods

Data source are the digital images obtained from the blood smears processed in the lab.
Data is analysed using image processing and machine learning techniques (e.g. convolutional neural networks (CNNs)).


## Challenges

This solution identifies the presence of platelet aggregates/microcoagulants responsible for a false decrease in the automated platelet count but does not perform an actual platelet count on the sample.
This project requires labs to have a slide scanner to digitalise the images used as data.

## What next?

The next step would be the optical count of platelets through the images used as data. 
In this way, as in addition to detecting the presence of platelet aggregates/microcoagulants, it would be possible to estimate the real number of platelets in the sample in combination with the data extracted from the automated complete blood count (CBC) and avoid to repeat the blood collection.

## Acknowledgments

* list here the sources of inspiration 
* do not use code, images, data etc. from others without permission
* when you have permission to use other people's materials, always mention the original creator and the open source / Creative Commons licence they've used
  <br>For example: [Sleeping Cat on Her Back by Umberto Salvagnin](https://commons.wikimedia.org/wiki/File:Sleeping_cat_on_her_back.jpg#filelinks) / [CC BY 2.0](https://creativecommons.org/licenses/by/2.0)
* etc

# Identification of pseudothrombocytopenia in blood smears


Final project for the Building AI course

## Summary
This project aims to detect the presence of platelet aggregates/microclots in peripheral blood smears, helping to distinguish between pseudothrombocytopenia and real thrombocytopenia in the medical laboratory.


## Background

Pseudothrombocytopenia consists of a false decrease in the platelet count and can be the result of EDTA (anticoagulant)-dependent platelet aggregation, microclots resulting from difficult or prolonged blood draws, cold agglutinins or improper handling of blood samples.
Due to the possible presence of platelet aggregates or microclots in the blood samples, automated platelet counting can be inaccurate, leading to potential misdiagnoses of thrombocytopenia.
When an automated platelet count is lower than the reference value or differs significantly from a previous result, microscopic examination of a blood smear is necessary to confirm the findings and this process can delay analytical results. As a biomedical scientist, I encounter this issue frequently in laboratory routine, where platelet count discrepancies must be validated by a qualified professional, further increasing the time required for accurate diagnosis.


## How is it used?

The process involves digitalising several images of the selected blood smears. Once the AI model is trained, it extracts features from these images to identify the presence of platelet aggregates or microclots.
If platelet aggregates or microclots are detected, the software flags the result and recommends re-confirming the platelet count using alternative methods (e.g., optical platelet counting) or suggests collecting a new sample with a different anticoagulant, such as sodium citrate. 
If no platelet aggregates or microclots are found, the result indicating thrombocytopenia is automatically validated.


## Data sources and AI methods

The data sources are the digital images obtained from the blood smears processed in the laboratory.
The analysis is carried out using image processing techniques and machine learning models, particularly convolutional neural networks (CNNs).

<img src="https://github.com/user-attachments/assets/07ecbc90-edc4-4b63-85d6-a04bf155af53" width="600">

<img src="https://github.com/user-attachments/assets/bdea7f8f-768f-4fdb-abe7-69628b130086" width="600">


## Challenges

While this solution successfully detects platelet aggregates or microclots, which are responsible for a false decrease in the automated platelet count, it does not perform an actual platelet count on the sample. Additionally, the implementation requires laboratories to have a slide scanner to digitalise the blood smear images.

## What next?

The next step would be to develop an optical platelet counting feature based on the digital images used for platelets aggregates/microclots detection. 
By combining this optical count with data from the automated complete blood count (CBC), it would become possible to estimate the real platelet count, reducing the need for repeat blood collections and further improving diagnostic accuracy.

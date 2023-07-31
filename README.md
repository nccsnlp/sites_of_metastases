# Sites of Metastatic Disease Inference (For internal sharing only)
This repository contains code implementation of Information Extraction (IE) System in the paper **Use of Natural Language Processing to Infer Sites of Metastatic Disease from Radiology Reports at Scale**. The IE system is made up of Named Entity Recognition Model, Assertion Status Detection Model, Relation Extraction Model and Post processing for term normalization. Note that these models are developed using Spark NLP library v3.4.2 and requires a Spark NLP Healthcare license. Please refer https://www.johnsnowlabs.com/spark-nlp-for-research-and-education/ on how to request for a free trial license.

### Links
[manuscript] (undergoing review)

### Setup
    For windows, you may refer windows_installation.pdf. Otherwise, please refer https://sparknlp.org/docs/en/install
    
### Software versions used
    java jdk8
    python 3.7.2 
    spark 3.1.2
    spark nlp 3.4.2

### Usage
Refer README.md in respective model folder on how to use the scripts. These codes are developed and tested in windows 11 environment.

### Acknowledgement
The notebooks are adapted from https://github.com/JohnSnowLabs/spark-nlp-workshop/tree/master/healthcare-nlp

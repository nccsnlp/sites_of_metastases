# Sites of Metastatic Disease Inference
This repository contains code implementation of Information Extraction (IE) System and Fine Tuning of Clinical LLMs for Multilabel Classification in the paper **Use of Natural Language Processing to Infer Sites of Metastatic Disease from Radiology Reports at Scale**. The IE system is a pipeline consisting of three models developed using the Spark NLP library version 3.4.2 and a post-processing step for term normalization. These three models are Named Entity Recognition Model, Assertion Status Detection Model and Relation Extraction Model. Note that these models required a Spark NLP Healthcare license for training/inference. Please refer https://www.johnsnowlabs.com/spark-nlp-for-research-and-education/ on how to request for a free trial license.

### Links
[manuscript] (undergoing review)

## For IE system
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

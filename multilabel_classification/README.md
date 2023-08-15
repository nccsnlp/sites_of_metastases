# Fine Tuning of Clinical LLMs for MultiLabel Classification of Sites of Metastases
Scripts to fine-tune transformer models for multilabel classification of Sites of Metastases for Radiology Reports (conclusion text) using simpletransformer/pytorch libraries.

## 1. create a new conda environment
```
    conda create -n pytorch_gpu python=3.7.2
    conda activate pytorch_gpu
```
## 2. install pytorch from:
- https://pytorch.org/ or https://pytorch.org/get-started/locally/


## 3. install following packages:
- simpletransformers: `pip install simpletransformers`

## 4. data preparation:
- csv files containing
```
    Text columns: conclusion
    Label column: true_site_of_mets (list of metastatic sites, eg ["site1","site2"])
```

## 5. run the training notebook
```
    simpletransformers_siteofmets_multilabel_bert
    pytorch_siteofmets_multilabel_gatortron 
```
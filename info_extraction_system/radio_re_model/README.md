After NER training, continue with Assertion/RE training.

Both Assertion/RE uses the same set of csv files.

## data folder: radio_re_model\dataset
## script folder: radio_re_model

## processing flow:
1. data preparation 
2. model training and evaluation
3. model inference

## [anaconda prompt]
	conda activate sparknlp
	cd dataset

## 1. data preparation
- prepare your csv files in the required format, see 02csv\csv_example
- only these columns are mandatory: relation,entity1,entity1_begin,entity1_end,chunk1,entity2,entity2_begin,entity2_end,chunk2

- place train csv file in dataset\02csv\csv_train
- place test csv file in dataset\02csv\csv_test
- Note that train file will be split into train/dev during spark nlp training.

- to preprocess/clean, 
	use jupyter notebook script: 02data_preprocessing. The generated output file allrelations.csv will also be used for assertion model training.

## 2. model training and evaluation
- to train/evaluate/run prediction pipeline, 
	use jupyter notebook script: 03train_radio_re_sites_of_mets

- check model performance (see re_result, re_output subfolders)

## 3. model inference
- use jupyter notebook script: 04predict_radio_re_sites_of_mets
- this notebook includes the post processing steps for term normalization

After NER training, continue with Assertion/RE training.

Both Assertion/RE uses the same set of csv files

## data folder: radio_assertion_model\dataset
## script folder: radio_assertion_model

## processing flow:
1. refer radio_re_model data preparation steps and copy the allrelations csv file from radio_re_model > dataset > 02csv folder
2. preprocess into training format, split into train/test by patient
3. model training and evaluation
4. model inference

## [anaconda prompt]
	conda activate sparknlp
	cd dataset
		
## 1. copy allrelations.csv files from radio_re_model>dataset>02csv folder

copy radio_re_model\dataset\02csv\allrelations.csv to 
radio_assertion_model\dataset\02csv

## 2. data preprocessing for train/test data (sparknlp assertion training data format)
- to preprocess/clean
	use jupyter notebook script: 00data_preprocessing

## 3. model training and evaluation
- to train/evaluate/run prediction pipeline
	use jupyter notebook script: 01train_radio_assertion
- check model performance (see assertion_result, assertion_output subfolders)

## 4. model inference
- use jupyter notebook script: 02predict_radio_assertion

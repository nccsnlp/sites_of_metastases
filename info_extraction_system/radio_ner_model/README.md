## data folder: radio_ner_model\dataset
## script folder: radio_ner_model

## processing flow:
1. data preparation (coNLL 2003 BIO format)
2. resample train set 
3. model training and evaluation
4. model inference

## [anaconda prompt]
	conda activate sparknlp
	cd radio_ner_model

## 1. data preparation
- prepare your conll file in coNLL 2003 BIO format
- see example conll file in dataset\02conll\conll_example\example.txt
- place train conll file in dataset\02conll\conll_train, eg train.txt
- place test conll file in dataset\02conll\conll_test, eg test.txt
- Note that train file will be split into train/dev during spark nlp training.

## 2. resample train sets (using oversample 'B'/'I' classes, undersample 'O' class)
- this is to address class imbalanced
- use jupyter notebook script: 02resample_trainsets to do the resampling. You may modify the resampling ratio to suit your dataset.
- train folder: 02conll\conll_train

## 3. model training and evaluation
- use jupyter notebook script: 03train_radio_ner_with_jsl_assertion_status
- train folder: 02conll\conll_train
- test folder: 02conll\conll_test
- check model performance (see ner_result, ner_output subfolders)

## 4. model inference
- use jupyter notebook script: 04predict_radio_ner

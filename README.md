## Code-Mixed Classification

This repository contains the source code for NLP course project.

![HIT](https://github.com/LCS2-IIITD/HIT-ACL2021-Codemixed-Representation/blob/main/image/model.png)

We publish the datasets (publicly available) and the experimental setup used for different tasks.

### Installation for experiments

	$ pip install -r requirements.txt

### Commands to run

#### Sentiment Analysis

	$ cd experiments && python experiments_hindi_sentiment.py \
			--train_data ../data/hindi_sentiment/IIITH_Codemixed.txt \
			--model_save_path ../models/model_hindi_sentiment/ --epochs 10
	$ cd experiments && python experiments_hindi_sentiment.py \
			--train_data ../data/hindi_sentiment/IIITH_Codemixed.txt \
			--model_save_path ../models/model_hindi_sentiment/ --mode test


#### PoS (Parts-of-Speech) Tagging 
	
	$ cd experiments && python experiments_hindi_POS.py \
			--train_data '../data/POS Hindi English Code Mixed Tweets/POS Hindi English Code Mixed Tweets.tsv' \
			--model_save_path ../models/model_hindi_pos/ --epochs 10
	$ cd experiments && python experiments_hindi_POS.py \
			--train_data '../data/POS Hindi English Code Mixed Tweets/POS Hindi English Code Mixed Tweets.tsv' \
			--model_save_path ../models/model_hindi_pos/ --mode test

#### Named Entity Recognition (NER)

    $ cd experiments && python experiments_hindi_NER.py\
    		--train_data '../data/NER/NER Hindi English Code Mixed Tweets.tsv' \
			--model_save_path ../models/model_hindi_NER/ --epochs 10
	$ cd experiments && python experiments_hindi_NER.py\
    		--train_data '../data/NER/NER Hindi English Code Mixed Tweets.tsv' \
			--model_save_path ../models/model_hindi_NER/ --mode test

			
#### Sarcasm Detection

	$ cd experiments && python experiments_hindi_SH.py \
			--train_data '../data/MSH-Comics-Sarcasm/hindi_sarcasm.txt' \
			--model_save_path ../models/model_hindi_sarcasm/ --epochs 10
	$ cd experiments && python experiments_hindi_SH.py \
			--train_data '../data/MSH-Comics-Sarcasm/hindi_sarcasm.txt' \
			--model_save_path ../models/model_hindi_sarcasm/ --mode test

#### Humour Classification

	$ cd experiments && python experiments_hindi_SH.py \
			--train_data '../data/MSH-Comics-Sarcasm/hindi_humour.txt' \
			--model_save_path ../models/model_hindi_humour/ --epochs 10
	$ cd experiments && python experiments_hindi_SH.py \
			--train_data '../data/MSH-Comics-Sarcasm/hindi_humour.txt' \
			--model_save_path ../models/model_hindi_humour/ --mode test
			
			
#### Response Prediction

	$ cd experiments && python experiments_response_prediction.py \
			--data_path '../data/IITMadras-CodeMixResponse/hindi' \
			--model_save_path ../models/model_hindi_response/ --epochs 10
	$ cd experiments && python experiments_response_prediction.py \
			--data_path '../data/IITMadras-CodeMixResponse/hindi' \
			--model_save_path ../models/model_hindi_response/ --mode test
			
#### Intent Detection

	$ cd experiments && python experiments_intent_detection.py \
			--data_path '../data/IITMadras-CodeMixIntent/GCN-SeA/hi-dstc2' \
			--model_save_path ../models/model_hindi_intents/ --epochs 10
	$ cd experiments && python experiments_intent_detection.py \
			--data_path '../data/IITMadras-CodeMixIntent/GCN-SeA/hi-dstc2' \
			--model_save_path ../models/model_hindi_intents/ --mode test

#### Slot Filling

	$ cd experiments && python experiments_slot_filling.py \
			--data_path '../data/IITMadras-CodeMixIntent/GCN-SeA/hi-dstc2' \
			--model_save_path ../models/model_hindi_slots/ --epochs 10
	$ cd experiments && python experiments_slot_filling.py \
			--data_path '../data/IITMadras-CodeMixIntent/GCN-SeA/hi-dstc2' \
			--model_save_path ../models/model_hindi_slots/ --mode test

#### ZSL pre-training
			
	$ cd experiments && python experiments_hindi_ZSL.py \
			--model_save_path ../models/model_hindi_zsl/ --epochs 10	

	$ cd experiments && python experiments_hindi_ZSL.py \
			--model_save_path ../models/model_hindi_zsl/ --mode test		
				

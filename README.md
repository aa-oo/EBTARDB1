# Event-Based-Time-Aware-Rumor-Detection-Benchmark
This repository is the official implementation of [Event-Based Time-Aware Rumor Detection
Benchmark]. 


## Requirements

To install requirements:

```setup
conda env create -f environment.yaml
```


## Training

To train the model(s) in the paper, run this command:

```train

BERT
cd Improving-Rumor-Detection-with-User-Comments-main
cd PHEME-RNR
python Rumor_BERT_domain_discriminator_data.py train event
cd TWITTER-RNR
python Rumor_BERT_domain_discriminator_data.py train event Twitter15

EANN
cd EANN-KDD18-master
cd src
python EANN_text_data.py train event
python EADD_text_twitter_data.py train event Twitter15

GACL
cd GACL-CADA
cd PHEME_two_classification
python main_pheme_domain_discriminator_data.py train b
cd Twitter_four_classification
python main_twitter_domain_discriminator_data.py train b Twitter15

MetaDetector
cd metadetector-master
cd src
python MetaDetector_data.py train event
python MetaDetector_Twitter_data.py train event Twitter15

```



## Pre-trained Models

Our pretrained models here:
BERT
Download from 'https://www.aliyundrive.com/s/S9RLpi5fERM' and place 'pheme' in BERT into Improving-Rumor-Detection-with-User-Comments-main/PHEME-RNR/model_all_domain
Download from 'https://www.aliyundrive.com/s/S9RLpi5fERM' and place 'twitter' in BERT into Improving-Rumor-Detection-with-User-Comments-main/Twitter-RNR/model_all_domain


EANN
Download from 'https://www.aliyundrive.com/s/S9RLpi5fERM' and place the files in EANN into EANN-KDD18-master/data/output/
EANN-KDD18-master/data/output/

GACL
GACL-CADA/PHEME_two_classification/model_all_domain
GACL-CADA/Twitter_four_classification/model_all_domain

MetaDetector
metadetector-master/data/output/


## Results

Our model achieves the following performance :
PHEME and PHEME-structure ![image](image/result_PHEME.png)
Twitter15 and Twitter16 ![image](image/result_Twitter.png)
Twitter15-structure and Twitter16-structure ![image](image/result_Twitter15-structure.png) [image](image/result_Twitter16-structure.png)




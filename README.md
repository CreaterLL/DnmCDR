# A Dynamic Cross-Domain Recommendation Model with Target-Aware Complementary Preference Transfer and Information Fusion
### introduction
This repository provides the implementations of DnmCDR.
### Requirements
Python 3.6

Pytorch 1.8

Tensorflow 2.6

Pandas

Numpy

Tqdm

### Dependent repositories
The implementation of the data processing and some baselines of our code are based on [PTUPCDR](https://github.com/easezyc/WSDM2022-PTUPCDR).​
### Dataset
The dataset used in DnmCDR is [Amazon Reviews 5-score dataset](http://jmcauley.ucsd.edu/data/amazon/links.html). Specifically, you can download them with following links:
1. [CDs and Vinyl](http://snap.stanford.edu/data/amazon/productGraph/categoryFiles/reviews_CDs_and_Vinyl_5.json.gz)
2. [Movies and TV](http://snap.stanford.edu/data/amazon/productGraph/categoryFiles/reviews_Movies_and_TV_5.json.gz)
3. [Books](http://snap.stanford.edu/data/amazon/productGraph/categoryFiles/reviews_Books_5.json.gz)

### Data preprocess
You can use the following command to preprocess the dataset. The two-phase data preprocessing includes parsing the raw data and segmenting the mid data. The final data will be under ./data/ready.

`python entry.py --process_data_mid 1 --process_data_ready 1`

### Training model

`python entry.py`

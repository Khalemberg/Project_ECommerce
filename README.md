# Olist Brazilian E-Commerce: Marketplace Analytics Notebook


This notebook contains the full analytical workflow for the project report. 

It addresses five tasks:
1. Explore the data and prepare it for analysis, with justification.
2. Discover product categories that are frequently purchased together.
3. Segment sellers by sales and service characteristics.
4. Identify unusual orders that merit operational review.
5. Predict (a) whether an order will arrive late and (b) how many days it will take from purchase to delivery.

### How to run this notebook

1. Download the dataset from Kaggle: <https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce>.
2. Unzip it and place the nine CSV files in a folder.
3. Library versions used:
  pandas       3.1.1
  numpy        2.5.5
  matplotlib   3.11.2
  seaborn      0.13.2
  scipy        1.18.1
  statsmodels  0.15.0
  sklearn      1.9.1
  mlxtend      0.25.0
   
4. ## 0. Set-up: imports and settings

All libraries are imported at the begining so that any missing package is reported straight away. A fixed random seed (`RANDOM_SEED = 42`) is used for every procedure that involves randomness (bootstrap resampling, k-means initialisation, random forests, Isolation Forest), so the results can be reproduced exactly.

5. Run all cells from top to bottom (*Kernel → Restart & Run All*). A full run takes roughly 10–15 minutes on a laptop, mostly in the random-forest tuning cells.

The notebook writes figures to a `figures` folder and summary tables to a `results` folder. Nothing needs to be done by hand between cells.
# ISE540FinalProject_4Drivers
This is the repository for the final project for ISE 540 of group 4 Drivers. It includes the code and the datasets for cars reviews analysis and rating prediction

## Cars Review Analysis and Rating Prediction 

CODE SCRIPTS

- 00 Web Scraping Edmunds.ipynb:
  - Script to collect the data from the website www.edmunds.com 
  - Data includes type, make, model, year of the car, as well as review (text), overall rating and aspects ratings

- 01 Data Processing & Cleaning.ipynb
  - Script to read in and clean the raw data scraped from Edmunds

- 02 Criteria Extraction.ipynb
  - Script extract the criteria/aspects from the text reviews 
    
    i) TF-IDF with K-Means Clustering method                                                                         
    ii) LDA analysis method

- 03 Classifiers.ipynb
  - Script to read in the manually labelled data and train classifications models to produce the aspects loadings for the whole dataset
  - Produces as output a dataset with aspect loadings for every text review that was scraped

- 04 Regression.ipynb
  - Script that takes as input the output of classifiers and fits regression models to predict the 5-star rating of the car based on the review

- 05 Evaluation.ipynb
  - Script that evaluates different regression models with different settings in terms of accuracy, precision, recall and f1 measure
  - Includes statistical significance testing for each of the models evaluated

DATASETS

- 01 initial_train_data_full_version.csv
  - Csv file containing the raw data that was scraped from www.edmunds.com. Csv file contains the columns type, make, model, year of the car, as well as total 5 star rating, the text review and the aspects 5 star rating

- 02 data_cleaned.csv
  - Csv file containing the output of the Data Processing & Cleaning script. From the original 22k rows, this csv file contains the 'cleaned' 18k rows

- 03 manual_labelling_data.xlsx
  - Excel file containing the 1000 rows sampled from the original data and the 9 discovered aspects with their manually labeled aspect loadings.

- 04 classifier_output_latest.csv
  - Csv file containing the output of the classification of the discovered outputs and the original dataset from edmunds. It is a sort of a 'full' dataset containing the original columns and the added columns from the classification. It is used for Regression and Models Evaluation

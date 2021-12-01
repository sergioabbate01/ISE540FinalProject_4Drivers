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

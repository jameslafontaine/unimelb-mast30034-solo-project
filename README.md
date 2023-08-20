# MAST30034 Project 1 README.md
- Name: `JAMES LA FONTAINE`
- Student ID: `1079860`

#####

**Research Goal:** My research goal is to analyse hourly taxi zone profitability and form predictions for use in routing / dispatch systems, and to provide insights to taxi drivers and taxi companies.

**Timeline:** The timeline for the research area is May-November 2022.

To run the pipeline, please visit the `notebooks` directory and run the files in order, running all cells from top to bottom unless otherwise specified:
1. `download.ipynb`: This downloads the data into the `data/landing` directory. Note that the census data .zip file has been included in the remote repository 
                     (data/landing) as the dataset is very small (couple of MB) and I was unable to get the Kaggle API to function correctly. The subway_entr_exit.csv file has also
                     been included as this file is also small and the download URL originally used doesn't appear to work anymore.
2. `preprocessing_part_1.ipynb`: This notebook details all landing->raw layer preprocessing steps and outputs it to the `data/raw` directory.
3. `preprocessing_part_2.ipynb`: This notebook details all raw->curated layer preprocessing steps and outputs it to the `data/curated` directory.
4. `data_analysis_imputation.ipynb`: This notebook is used to perform imputation on the combined data.
5. `data_analysis_geospatial.ipynb`: This notebook is used to conduct geospatial analysis on the combined data.
6. `data_analysis_temporal.ipynb`: This notebook is used to conduct temporal analysis on the combined data.
7. `data_analysis_external.ipynb`: This notebook is used to conduct external dataset feature analysis on the combined data.
8. `modelling_linregression.ipynb`: This notebook is used to fit/tune linear regression models.
9. `modelling_xgboost.ipynb`: This notebook is used to fit/tune xgboost models. Note that the hyperparameter tuning cells may take a while to run if desired.
10. `modelling_comparison.ipynb`: This notebook is used to compare the the linear regression and xgboost models.

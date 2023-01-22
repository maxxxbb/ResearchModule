# Final Project: Research Module: Applied Microeconomics
### Authors

- Maxie Schulze (University of Bonn)
- Lara Schorer (University of Bonn)
- Mehmet Emir Kavukcu (University of Bonn)
- Max Boehringer (University of Bonn, s6mxboeh@uni-bonn.de)



### About

In this study, we examine the relationship between negative reciprocity preferences, unfair treatment and turnover intentions using large-scale survey data from the German Socio-Economic Panel Study (SOEP). We apply a linear probability model to analyze the data and find that higher measures of negative reciprocity and missing recognition at the workplace are linked to higher turnover intentions. However, we do not find any conclusive evidence in the data that the effect of unfair treatment on turnover intentions is stronger for individuals with higher levels of negative reciprocity. The results are robust to different robustness checks. We discuss possible explanations, such as measurement errors in the reciprocity variable or unobserved factors related to both the predictor and the outcome variable.

This repository contains scripts for all data cleaning and analysis to replicate the results of the paper:


### Requires
In order to run this project on your local machine you need to have installed Python, an Anaconda distribution and LaTex distribution in order to compile .tex documents.
You further need access to the SOEP-Core dataset and insert its filepath into the scripts.

The project was created on Windows 10 using

- Anaconda 4.11.0
- Python 3.9.10

All necessary python dependencies are contained in environment.yml . To install the virtual environment in a terminal move to the root folder of the repository and type `$ conda env create -f environment.yml` and to activate type  `$ conda activate replication_ar2018`.

### Content

For this project we worked in .ipynb files, thus all regression outputs can be examined without running the code on your local machine on Github. All scripts are inside the `src/data_management` folder.

- Absenteism.ipynb : Analysis for outcome job-effort proxied by absent days from work
- Addpeople.ipynb : Creates .csv with 2006 controls
- AddpeopleERI.ipnyb : Creates .csv with 2006 controls and calculates Effort-Reward-Ration for each individual (Robustness Check)
- Addpeoplepositive : Creates .csv with 2006 controls and measures for positive reciprocity preferences
- changes_of_reciprocity_measure : Check whether reciprocity preferences are stable over the survey years
- Effort-Reward-Imbalance : Analysis with ERR-Ratio (Robustness Check)
- FirstRegression : Main notebook. Contains functions to read in and clean data. Contains Results for all Robustness Checks
- job_satisfaction.ipnyb: Analysis for outcome job satisfaction
- Positive_reciprocity.ipynb : Analysis with measures for positive reciprocity and recoded treatment
- regression_effort.ipynb : Analysis for outcome job-effort proxied by overtime work
- papernotfinal.pdf : not so final paper
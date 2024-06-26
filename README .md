Project Title: Analysis of the Fox Insight Parkinson's Dataset

Project Overview
This project involves the analysis of the Fox Insight Parkinson's Dataset to uncover subtypes of Parkinson's disease, identify significant factors in treating the disease, and predict the diagnosis of Parkinson's disease using supervised and unsupervised methods.

Authors
Aswin Guvvala (aguvvala@depaul.edu)
Wei Tong Su (wsu6@depaul.edu)
Michael Ruggeri (mruggeri@depaul.edu)
Abstract
The Fox Insight Parkinson’s Dataset provides extensive data from patients fighting Parkinson’s disease, collected through various questionnaires. This project employs both supervised and unsupervised methods to analyze the data, identify disease subtypes, assess the impact of cannabis use on symptoms, and predict Parkinson's diagnosis.

Data Sources
PD-PROP 2.0 dataset: Contains 14 domains where patients rank the botherness caused by symptoms.
Cannabis Use in PD dataset: Information on THC and CBD dosage.
General dataset: Contains information about whether a patient has Parkinson’s Disease.
Methodology
Data Merging and Cleaning: Merged data from three CSV files (Cannabis_Use_in_PD.csv, PDPROP2.csv, General.csv) using fox_insight_id as the key, and cleaned the dataset by handling NaN values and transforming relevant columns.
Feature Engineering: Created new features from existing data, including binary indicators for cannabis use and symptom botherness.
Clustering: Applied clustering techniques, specifically mini-batch k-means, to define subtypes of Parkinson’s disease.
Logistic Regression: Developed logistic regression models to assess the impact of cannabis use, age, and Parkinson's diagnosis on various symptoms.
Results
Cannabis Use: Cannabis was found to aid in sleep, with CBD showing a positive relationship with sleep botherness.
Age and Symptoms: Age negatively correlated with all dependent variables (cognition bother, motor symptoms bother, pain bother, sleep bother, and Bradykinesia bother).
Parkinson's Diagnosis: Current diagnosis had a positive relationship with motor symptoms botherness.
Clustering: Mini-batch k-means provided the best clustering results for subtyping Parkinson’s disease.
Conclusions
Age and Parkinson's Diagnosis: Significant factors in predicting symptom botherness.
Cannabis Use: Particularly CBD, may impact sleep bother.
Future Work: Suggests exploring LSTM models for the longitudinal data and refining the data for better ergonomic use by non-analysts.
Contributions
Clustering Analysis: Michael and Wei
Regression Model for Cannabis Use: Aswin
Term Frequency Matrix of Questionnaire Text Files: Michael
References
Fereshtehnejad, Seyed-Mohammad et.al. (2017). Clinical Criteria for Subtyping Parkinson’s Disease: Biomarkers and Longitundinal Progression. Brain, Journal of Neurology.
Maaten, Laurens van der, Geoffrey Hinton. (2008). Visualizing Data Using t-SNE. Journal of Machine Learning Research, 9, 2579-2605.
Parkinson’s disease information: NIA, NHS

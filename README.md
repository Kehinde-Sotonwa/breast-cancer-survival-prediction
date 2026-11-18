Breast Cancer Survival Prediction Using Machine Learning

Project Overview

This repository contains the experimental implementation for evaluating machine learning models for breast cancer survival prediction using the METABRIC dataset.

The study evaluates five individual machine learning classifiers and a soft-voting ensemble using repeated stratified five-fold cross-validation.

Models Evaluated

Logistic Regression

Random Forest

XGBoost

LightGBM

CatBoost

Soft Voting Ensemble (XGBoost, LightGBM and CatBoost)

Experimental Methodology

Repeated stratified five-fold cross-validation with two repetitions.

Data scaling using StandardScaler within each training fold.

Class balancing using SMOTE within each training fold.

Evaluation using accuracy, sensitivity, specificity, precision, F1-score and ROC-AUC.

Results reported as mean and standard deviation across ten evaluation folds.

Corrected paired resampled t-test for comparing the ROC-AUC of the Voting Ensemble and CatBoost.

Computational Environment

Operating system: Linux

Python: 3.13.18

Processor: x86_64, 2 logical CPU cores

RAM: 12.67 GB

GPU: Not available (CPU execution)

Scikit-learn: 1.6.1

Imbalanced-learn: 0.14.2

XGBoost: 3.4.1

LightGBM: 4.6.0

CatBoost: 1.2.10

Dataset

The METABRIC dataset was used for the experiments. The patient-level dataset is not included in this repository.

Users intending to reproduce the experiment must obtain the dataset through its appropriate access arrangements and provide the required CSV files in the Google Drive folder specified in the notebook.

Running the Experiment

Open the experimental Jupyter notebook in Google Colab.

Obtain the required METABRIC dataset files.

Place the files in the Google Drive directory specified in the notebook.

Install the required Python libraries.

Run the notebook cells sequentially.

Repository Contents

Comment_3_Reproducibility_Experiment_BC_Survival_Repeated_CV_Corss Validation_NOV182026.ipynb: Experimental code for repeated cross-validation and statistical comparison.

README.md: Project description and reproduction instructions.

requirements.txt: Required Python libraries and versions.

Reproducibility

The notebook provides the experimental procedures, model configurations, evaluation metrics and computational environment used in the study.

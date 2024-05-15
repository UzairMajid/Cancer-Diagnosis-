# Gene-classfication-for-cancer-prediction
---
## Introduction
---
This use case deals with the classification of Gene classification for Cancer detection.The aim was to develop ML algorithms to classify genetic mutations based on clinical evidence (text). There are nine different classes for classification. This task is complex due to the challenging nature of interpreting clinical evidence, even for human specialists. The clinical evidence (text) is crucial for successful classification.

we have training and test datasets through two files: one for genetic mutations (training/test_variants) and another for clinical evidence (training/test_text). These files are linked by an ID field. For example, the genetic mutation with ID=15 in training_variants is classified using the clinical evidence from the row with ID=15 in training_text.

## Summary:
---
We first set up a baseline model which we can then compare with the other models. The baseline was simply a random classifier which randomly outputed the labels. 
We then used the below ML models:
1. Knn
2. Naive Bayes
3. Logistic Regression with and without class balancing
4. Support Vector Machines
6. Random Forest.

We used Platt's calibration to calibarte the probabilities.

### Evaluation Metrics:

Since our training data is imabalanced,  to evaluate the different models, we used the below metrics:
1.Precision
2. Recall

### Performance Comparision
Out of all the models, logistic regression with class balancing acheived lowest log loss:1.031190254308968

## Directories
---
The project is structured as follows:

bin: This directory contains the source code files required to run the analysis.

1. unet-eda-and-modelling-baseline: This Python notebook is the main entry point for executing the project. It contains the code that reads the dataset and performs various data processing, modelling and visualization tasks.
1. 2. unet-tesing-and-predictions: This Python notebook demonstrates the testing and prediction phase for the constructed Unet model.
scripts: This directory contains the script of models used for this projects (Baseline and superior Unets).

plots: This directory contains the plots produced during this project.

## User Guide
---
To use this project, follow the steps below:

1. Clone the repository: git clone https://github.com/UzairMajid/Gene-classfication-for-cancer-prediction

2. Install the required dependencies: pip install -r requirements.txt

3. Download the dataset from here https://www.kaggle.com/competitions/msk-redefining-cancer-treatment/data.
4. Run the mentioned notebook

## Contact Information
---
For any questions, suggestions, or issues, please feel free to contact:

Name: Uzair Majid

Email: majid@uni-potsdam.de


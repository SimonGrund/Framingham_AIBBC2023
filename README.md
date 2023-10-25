# Framingham_AIBBC2023
Cardiovascular Health Analysis With The Framingham Data Set

## Introduction
The Framingham Heart Study is an ongoing study of cardiovascular health of residents of the city of Framingham, Massachusetts. The study includes measurements of several potential biomarkers of cardiovascular disease and has laid the foundation to much of our current understanding of associations between lifestyle and health. 

## Data
We have included the first-generation Framingham data set in the data set folder, along with a subset of five hundred individuals that you can use to evaluate code on a small subset before using it on the full data. The data is also accessible directly through R:

install.packages("riskCommunicator")
d = data("framingham", package="riskCommunicator")

## Potential questions
- How many individuals are in the data?
- How many men and women, and what ages?
- How do the biomarkers correlate?
- Can you separate gender by unsupervised cluster analysis and/or dimension reduction?
- Can you train a supervised model that differentiates between individuals that reached cardiovascular disease (chdfate == T) and those that did not?
    - Evaluate model performance on a held-out test set
    - Evaluate model performance using cross-validation
    - Regularize a model to identify the optimal set of included biomarkers

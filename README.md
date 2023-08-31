# cross-class-validation
a cross-validation approach to finding out-of-distribution uncertainty thresholds for open-set recognition.

## Introduction
This repository holds the code for the final project of the graduate course "Statistical Machine Learning" at the computer engineering department of Sharif University of Technology. The goal of the project is to apply open-set recognition to the Oxford-102 dataset. We first implemented several uncertainty estimation methods, some of which were our own ideas. To get an estimation of what constitutes an out-of-distribution threshold, we developed the "cross-class-validation" approach. The approach consists of:

1. Putting aside one of the seen classes.
2. Finding the threshold that best separates the separated class from the available seen classes (F1 score is used here to find the threshold with the highest in and out-of distribution detection accuracy).
3. The process is repeated for all classes to find the threshold with the best average F1 accuracy across all classes.

We then applied Bayesian nonparametric approaches such as the Bayesian GMM with a Dirichlet prior to clustering the unseen data. 

## Results

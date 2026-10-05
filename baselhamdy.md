#### Baselhamdy - 500 Days of Software

#### Week 3

`Day18 oct 4, 2026`

- Learned the confusion matrix
- Learned sensitivity and specificity
- Learned ROC and AUC
- Learned cross validation
- Ran code for the classification metrics (sections 5-8 of `sklearn_classification_reference.ipynb`) and changed the threshold to see how the results change

`Day19 oct 5, 2026`

1.Videos :

Inria scikit-learn MOOC: "Validation of a model"
Inria scikit-learn MOOC: "Visualizing scikit learn pipelines in Jupyter"

2.Credit Risk Project :

Found special codes (96 and 98) in 269 rows of the late-payment columns. These rows default 54.6% of the time, so I kept a flag and replaced the codes with NaN
Only 6.7% of the rows default, so accuracy is a bad metric. I did a stratified split to keep this rate in train and test

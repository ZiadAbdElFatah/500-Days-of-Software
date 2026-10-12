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

-Inria scikit-learn MOOC: "Validation of a model"
-Inria scikit-learn MOOC: "Visualizing scikit learn pipelines in Jupyter"

2.Credit Risk Project :

-Found special codes (96 and 98) in 269 rows of the late-payment columns. These rows default 54.6% of the time, so I kept a flag and replaced the codes with NaN
-Only 6.7% of the rows default, so accuracy is a bad metric. I did a stratified split to keep this rate in train and test

`Day20 oct 6, 2026`

Credit Risk Project:
- Add pipeline (median imputer, scaler, logistic regression)
- Add baseline (most frequent class)
- Add 5-fold stratified CV with ROC AUC, recall, precision
- Add HistGradientBoosting and compare on the same folds
- Choose threshold 0.136 on out-of-fold probabilities (recall target 0.60)
- Run final test once on X_test (ROC AUC 0.8676, recall 0.611, precision 0.326)
- Add README

`Day21 oct 7, 2026`

GSoC Research :
- Read the NumFOCUS GSoC 2026 list. PyMC, Matplotlib, sbi, SciML and PyTorch-Ignite are all on it
- Read the ideas pages of PyMC, sbi and PyTorch-Ignite
- sbi and PyMC fit best. Both need a small PR to apply
- PyTorch skills must come earlier for sbi

`Day22 oct 8, 2026`
BREAK

`Day23 oct 9, 2026`
BREAK

#### Week 4

`Day 24 Oct 10, 2026`
BREAK

`Day 25 Oct 11, 2026`

Videos :
- Neural networks started from the idea of copying the brain, but they are only loosely related to it
- Inputs go through hidden units, and each unit computes one new feature
- Early layers find simple things like edges, and later layers find bigger things like faces
- A layer is a group of neurons, and it outputs a vector a
- Each neuron computes a = sigmoid(w·x + b)
- a[l] is the output of layer l, and it is the input of layer l+1
- Forward propagation moves data from x to the output, one layer at a time
- In the lab, I built single neurons and layers in code

`Day26 oct 12, 2026`

1.Videos :

-Andrew Ng ML Specialization: "Inference in Code"
-Andrew Ng ML Specialization: "Data in TensorFlow"
-Andrew Ng ML Specialization: "Building a Neural Network"

2.What I Learned :

-I can build a layer with `Dense(units=3, activation='sigmoid')`, call it on `x` to get `a1`, and pass `a1` to the next layer. TensorFlow uses matrices, so one example is `[[200.0, 17.0]]`, and `.numpy()` converts a tensor to a NumPy array
-`Sequential([layer_1, layer_2])` joins the layers. Then `compile` sets the loss, `fit` trains, and `predict` does inference

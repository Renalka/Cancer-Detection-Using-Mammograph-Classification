# Cancer-Detection-Using-Mammograph-Classification

Using real world data of masses detected in mammograms to determine whether or not those masses are benign or malignant in nature.

We have used supervised classification machine learning techniques and pitted them against each other. Based on its measurements using multiple different classification techniques we see which one does the best.

Predicting whether a mass shown in a mammogram is benign or malignant
Dataset used : "mammographic masses" public dataset from the UCI repository (source: https://archive.ics.uci.edu/ml/datasets/Mammographic+Mass)

This data has 961 rows and the following attributes:

BI-RADS assessment: 1 to 5 (ordinal)
Age: patient's age in years (integer)
Shape: mass shape: round=1 oval=2 lobular=3 irregular=4 (nominal)
Margin: mass margin: circumscribed=1 microlobulated=2 obscured=3 ill-defined=4 spiculated=5 (nominal)
Density: mass density high=1 iso=2 low=3 fat-containing=4 (ordinal)
Severity: benign=0 or malignant=1 (binominal)
BI-RADS is an assesment of how confident the severity classification is; it is not a "predictive" attribute and so we will discard it. The age, shape, margin, and density attributes are the features that we will build our model with, and we will try to predict the "severity" based on those attributes.

Although "shape" and "margin" are nominal data types, they are close enough to ordinal, hence we will not just discard them. The "shape" for example is ordered increasingly from round to irregular.

Our approach
We will apply different supervised machine learning techniques to this dataset and model evaluation will be done using K-Fold cross validation (K=10).

Decision tree
Random forest
KNN
Naive Bayes
SVM
Logistic Regression
Neural network using Keras

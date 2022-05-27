Sequence Models
===============

This mini-course is designed to give you a hands-on introduction to classic
sequence models used in bioinformatics. It is expected that you have some
previous knowledge in:

+ Unix/Linux command line
+ Programming in Python
+ Molecular biology

Setup
-----

All of the example code is 100% Python using minimal externaal dependancies.
However, there are a few libraries you will have to install. It is recommended
that you use Conda or other package maintainer and not install directly into the
base Python of your OS.

+ `pip3 install numpy`

Data
----

Data included here:

+ Proteins - for regex, but how to define positives and negatives?
+ Splice sites
+ Exons and introns


Measures of Accuracy
--------------------

We are going to be comparing a variety of sequence models. Towards this end, we
need a common way to assess the performance of each. There are standar formulae
for doing this, all of which are based on 4 values.

+ TP - true positives
+ FP - false positives
+ TN - true negatives
+ FN - false negatives

The are many ways to aggregate these numbers to summarize performance. Here are
a few:

+ True Positive Rate (sensitivity): TPR = TP / (TP + FN)
+ True Negative Rate (specificity): TNR = TN / (TN + FP)
+ Positive Predictive Value (precision): PPV = TP / (TP + FP)
+ False Discovery Rate: FDR = FP / (FP + TP)
+ Accuracy: ACC = (TP + TN) / (TP + TN + FP + FN)
+ F1 score: F1 = 2TP / (2TP + FP + FN)

Which is the best way to evaluate a discriminator? There is no single best way
but a bad way is to focus on one. For example, it is easy to optimize
sensitivity and end up with terrible specificity and vice-versa.

Regular Expressions
-------------------

+ Canonical signals
	+ ATG
	+ GT..AG
+ Concensus sequence
	+ GTRAG
	+ HOMER PWMs to find examples
+ Regular expression
	+ PROSITE
	+ Converting concensus to regex


Decision Tree
-------------



Position Weight Matrices
------------------------


Markov Models
-------------

Weight Array Matrices
---------------------


Hidden Markov Models
--------------------

Support Vector Machine
----------------------


Perceptron
----------


Multi-layer Perceptron
----------------------



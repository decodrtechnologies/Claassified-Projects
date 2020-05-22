# DIMENSIONALITY REDUCTION

Dimensionality reduction is the process of reducing the number of random variables under consideration by obtaining a set of principal variables.

## PRINCIPAL COMPONENT ANALYSIS(PCA)

### UNSUPERVISED LINEAR FEATURE PROJECTION

PCA is mostly used as a tool in exploratory data analysis and for making predictive models. It is often used to visualize genetic distance and relatedness between populations.

### Steps :

> * Organize data as an m×n matrix, where m is the number of measurement types and n is the number of samples.
> * Subtract off the mean for each measurement type.
> * Calculate the SVD or the eigenvectors and eigen value of the covariance.
> * Now the eigen value with higher value corresponds to eigen vector with high variance.
> * Only use those dimension which contain maximum information(ie high eigen values)

### Content :
> * Feature selection
> * Feature extraction
> * Advantages of dimensionality reduction
> * PCA
> * Practical implementation : Wholesale Customer dataset

### Data :

We will be using a [Wholesale customers dataset](https://archive.ics.uci.edu/ml/datasets/Wholesale+customers#) 
from the [UCI Machine learning repository](https://archive.ics.uci.edu/ml/index.php) which has a very good collection of datasets.

Features used in this project:
- FRESH
- MILK
- GROCERY
- FROZEN
- DETERGENTS_PAPER
- DELICATESSEN

**Source :**

Margarida G. M. S. Cardoso, margarida.cardoso '@' iscte.pt, ISCTE-IUL, Lisbon, Portugal

### License : 
This is an opensource dataset which can be found on UCI Repository.

Citation :
Abreu, N. (2011). Analise do perfil do cliente Recheio e desenvolvimento de um sistema promocional. Mestrado em Marketing, ISCTE-IUL, Lisbon

Dua, D. and Graff, C. (2019). UCI Machine Learning Repository [http://archive.ics.uci.edu/ml]. Irvine, CA: University of California, School of Information and Computer Science.

@misc{Dua:2019 ,
author = "Dua, Dheeru and Graff, Casey",
year = "2017",
title = "{UCI} Machine Learning Repository",
url = "http://archive.ics.uci.edu/ml",
institution = "University of California, Irvine, School of Information and Computer Sciences" }


### Requirements :

You will also need to have software installed to run and execute a [Jupyter Notebook](http://ipython.org/notebook.html)

If you do not have Python installed yet, it is highly recommended that you install the [Anaconda](http://continuum.io/downloads) distribution of Python, which already has the above packages and more included. 

This project requires **Python** and the following Python libraries installed:

- [NumPy](http://www.numpy.org/)
- [Pandas](http://pandas.pydata.org/)
- [Matplotlib](http://matplotlib.org/)
- [Scikit-learn](http://scikit-learn.org/)

### Run :

In a terminal or command window, navigate to the top-level project directory `PCA Dimensionality Reduction/`
(that contains this README) and run one of the following commands:


ipython notebook PCA_Dimension_reduction_solution.ipynb
or

jupyter notebook PCA_Dimension_reduction_solution.ipynb


This will open the Jupyter Notebook software and project file in your browser.



# DIMENSIONALITY REDUCTION

Dimensionality reduction is the process of reducing the number of random variables under consideration by obtaining a set of principal variables.

## t-SNE(t-distributed stochastic neighbor embedding) 

### UNSUPERVISED NON LINEAR FEATURE PROJECTION

t-SNE (t-Distributed Stochastic Neighbor Embedding) is an algorithm used for dimensionality reduction. It is used for high dimensional datasets (images for example).
It is more expensive than PCA and LDA but it gives better results for complex data as you will see below.    
Reference to understand algorithm : [t-SNE](https://www.youtube.com/watch?v=NEaUSP4YerM)

### Drawbacks :

- It is highly recommended to use another dimensionality reduction method (e.g. PCA for dense data or TruncatedSVD for sparse data)to reduce the number of dimensions to a reasonable amount (e.g. 50)if the number of features is very high.
- Since t-SNE scales quadratically in the number of objects N, its applicability is limited to data sets with only a few thousand input objects; beyond that, learning becomes too slow to be practical (and the memory requirements become too large

### Steps :

> * Compute similarity matrix between all feature vectors
> * Compute similarity matrix from map points
> * Use gradient descent to minimimze distance between matrices

### Data :

We will be using a [pokemon dataset](https://www.kaggle.com/abcsds/pokemon) from the kaggle which has a very good collection of datasets.

Features used in this project:
- #
- Name
- Type 1
- Total
- HP
- Attack
- Defense
- Sp. Atk
- Sp. Def
- Speed
- Generation
- Legendary

### [License](https://creativecommons.org/publicdomain/zero/1.0/) : 
This is an opensource dataset which can be found on kaggle platform.


### Requirements :

You will also need to have software installed to run and execute a [Jupyter Notebook](http://ipython.org/notebook.html)

If you do not have Python installed yet, it is highly recommended that you install the [Anaconda](http://continuum.io/downloads) distribution of Python, which already has the above packages and more included. 

This project requires **Python** and the following Python libraries installed:

- [NumPy](http://www.numpy.org/)
- [Pandas](http://pandas.pydata.org/)
- [Matplotlib](http://matplotlib.org/)
- [Seaborn](https://seaborn.pydata.org/)
- [Scikit-learn](http://scikit-learn.org/)

### Run :

In a terminal or command window, navigate to the top-level project directory `t-SNE Dimensionality Reduction/`
(that contains this README) and run one of the following commands:


ipython notebook tsne_task.ipynb
or

jupyter notebook tsne_task.ipynb


This will open the Jupyter Notebook software and project file in your browser.



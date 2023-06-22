<a target="_blank" href="https://colab.research.google.com/github/Skalwalker/AntiMoneyLaundering/blob/main/anti_money_laundering.ipynb">
  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
</a>

# AntiMoneyLaundering
Classify Money Transactions in the "IBM Transactions for Anti Money Laundering" Dataset


## Project Description
The project is based on the analysis of the «IBM Transactions for Anti Money Laundering» dataset published on Kaggle and released under the Community Data License Agreement – Sharing – Version 1.0. This dataset contains several CSV files, each having a different combination of data size and amount of illicit transactions. It is up to you to choose the files to be considered in your analysis. If needed, you can subsample any such file (i.e., consider a subset of the available attributes or a subset of the items to be processed, or both).

## Tasks

The task is to implement a system which predicts whether or not a transaction is illicit, using the attribute "Is Laundering" as a label to be predicted. Classification should be done exploiting a random forest, organizing the project as follows.

1. A sequential implementation (from scratch) of the learning algorithm for a decision tree should be provided, and tested using one or more subsets of the dataset which can be loaded in main memory.
2. A mock-up code that uses spark in order to consider a dataset and processes it in order to distribute the creation of the single trees in a random forest should be proposed. In particular, the construction of each tree should be done by providing different data to each worker,, both subsampling the number of rows (i.e., labeled objects) and columns (i.e., attributes) in the overall dataset. Concerning the first kind of subsampling, you might possibly consider introducing the so-called bootstrap sampling, in which the labeled objects are sampled with replacement and therefore a same object can occur more than once in the resulting dataset. It is not required to distribute the creation of a single decision tree: for this task you are free to use the implementation provided in point 1, as well as the implementation already available in scikit-learn.

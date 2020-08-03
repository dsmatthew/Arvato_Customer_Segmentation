# Arvato_Customer_Segmentation
Project about the Kaggle challange in corporation with Udacity

### Table of Contents

1. [Installation](#installation)
2. [Project Motivation](#motivation)
3. [File Descriptions](#files)
4. [Results](#results)
5. [Licensing, Authors, and Acknowledgements](#licensing)

## Installation <a name="installation"></a>

You need to have a Python 3.x environment. I used anaconda. This project uses some packages, which you might need to install using the statement "pip install my_package" in your conda console.

Used special packages:
* h2o v3.30.0.7 (auto machine learning library - https://pypi.org/project/h2o/)
* kneebow v0.1.1 (exctracting the optimal value by elbow strategy - https://pypi.org/project/kneebow/)

Used libraries:
* numpy
* pandas
* matplotlib
* seaborn
* scipy
* sklearn
* pickle

## Project Motivation<a name="motivation"></a>

Arvato published data sets to find machine learning model for predicting which customers is more likely to respond to the selected campaign.
In this project I will investigate characteristics in a general population data set versus the customers data set. This is done by applying unsupervised learning methods. The second step will be to create a supervised learning model to predict customers who are more likely to react on the mail out campaign by the company.
All data sets are provided by Arvato (via Kaggle) in corporation with Udacity (www.udacity.com).



## File Descriptions <a name="files"></a>
* data sets - due to legal terms, you have to access the files by yourself via Udacity Nanodegree
 * Udacity_AZDIAS_052018.csv - unlabeled data set for clustering
 * Udacity_CUSTOMERS_052018.csv - unlabeled data set for clustering
 * Udacity_MAILOUT_052018_TEST.csv - unlabeled data set for prediction & submission for Kaggle (https://www.kaggle.com/c/udacity-arvato-identify-customers/overview)
 * Udacity_MAILOUT_052018_TRAIN.csv - labeled data set for supervised model training
 * DIAS Attributes - Values 2017.xlsx - information about columns
 * DIAS Information Levels - Attributes 2017.xlsx - information about leves of the columns
* Arvato Project Workbook.ipynb contains the analysis with output written in python and used in Jupyter Notebook / Jupyter Lab
* model_kmeans.pkl The trained k-means clustering model, which is applied for Part II & Part III (supervised learning)
* model_h2o_automl_leader/* h2o models which were trained an applied in Part II & Part III (supervised learning)

## Results<a name="results"></a>

The findings to the previously defined business questions are discussed in this [blogpost on medium](http://google.com)

Short conclusion:
The given data sets are analyzed using data analytics methodologies. In the first part several findings about the two data sets (general population sample compared to customers data set) lead to the clustering into 14 clusters. On basis of these findings, a supervised model is built. The model performance should be improved in future iterations. These could be:
* Implementing more custom imputation strategies
* Deriving new features by using the feature importance of the GBM or PCA weights
* Testing more algorithms and/or a larger parameter grid



## Licensing, Authors, Acknowledgements<a name="licensing"></a>
I used the data from Arvato BERTELSMANN provided by Udacity within their Nanodegree. All the licensing for the data and other information can be found on [Udacity](https://udacity.com)

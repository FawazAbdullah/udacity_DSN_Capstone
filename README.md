# Sparkify data analysis

This project is the analysis of a dataset that contains user logs for a music streaming service called "Sparkify" (no need to search for it it does not exist). This is my submission to the capstone project of the Udacity data scientist nanodegree.

The Sparkify music service looks to identify the population of users that churn (they can be users from the free service, or the paid service). Once the possible criteria for churn are better undestood, our objective is to build a model and predict the users churn so that some specific attention can be given to the users and try to retain them on the platform.

The repository contains only the jupyter notebook, without the data files. Data files are available from the Udacity nanodegree platform.  The provided dataset contains the logs of the user actions (pages seen by users along with other encoded properties such as location, time, operating system used, subscription level of the user for example).

The notebook goes through the following sections to easily allow a reader to follow the data understanding and modeling steps I went through:
- Load and Clean Dataset
- Exploratory Data Analysis
  - Define Churn
  - Explore Data
- Feature Engineering
- Modeling
- Conclusion


## Installation <a name="installation"></a>

The additional libraries on top of the standard distribution of Python 3.* necessary are:
- matplotlib: https://matplotlib.org/ (for data visualisations)
- seaborn: https://seaborn.pydata.org/ (for data visualisations)
- pandas: https://pandas.pydata.org/ (for processing some smaller datasets)
- pyspark: https://spark.apache.org/ (for processing the sparkify dataset which can be too big to fit in memory of a single machine)


## Project Motivation<a name="motivation"></a>

The reason for creating this project is to submit the Udacity nanodegree capstone project as a final validation of the nano-degree. I enjoyed discovering pyspark to handle large datasets.


## File Descriptions <a name="files"></a>

This repository contains the following files:
- [README.md](README.md): this file
- [Sparkify.png](Sparkify.png): screenshot taken from a video describing the sparfiky service and used as an image illustrating the blog post
- [Sparkify.ipynb](Sparkify.ipynb): jupyter notebook that contains the whole data analyis process


## Results<a name="results"></a>

As a summary, the small dataset used in this notebook allowed me to engineer a total of 13 features that look like they are able to predict the user churn. I was able to run 4 different classifier models, and tune those that gave the highest F1 score. Then I ran the best model (which turned out to be the Multilayer Perceptron classifier) on the validation set and eventually got 79.2% accuracy on the validation set.

A longer description of the findings in the data can be found at the post available [here](https://medium.com/@stephaneschitter/how-to-predict-churn-of-sparkify-users-834bc5de4ffe).


## Licensing, Authors, Acknowledgements<a name="licensing"></a>

Credits go to Udacity for making the data available.

Feel free to use the code from the notebook for your own purposes.
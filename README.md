
# Starbucks Capstone Challenge
![](https://cdn.shortpixel.ai/client/q_lossy,ret_img,w_924/https://wichitaonthecheap.com/lotc-cms/wp-content/uploads/Starbucks-Happy-Hour-2.jpg)

## Table of Contents
1. [Installation](#Installation)
2. [Project Motivation](#Project)
3. [File Description](#Description)
4. [Licensing, Authors, Acknowledgements](#License)
5. [Summary](#Summary)

## <a name="Installation"></a>Installation
There should be no libraries necessary to run the code here beyond the Anaconda distribution of Python. The code should run with no issues using Python versions 3.*.

## <a name="Project"></a>Project Motivation
This data set provided by Starbucks, contains simulated data that mimics customer behavior on their rewards mobile app. Once every few days, Starbucks sends out an offer to users of the mobile app. An offer can be merely an advertisement for a drink or an actual offer such as a discount or BOGO (buy one get one free). The goal of this project is to analyze how well certain customer groups respond to certain offer types by combining the three provided data sets. In order to achieve this goal, I had to clean and combine the three provided data sets first and then explore the data by visualizing it. Then the data was modeled, to be able to determine if an offer was viewed and then completed by am member. At the end, I used a GradientBoostingClassifier in combination with GridSearchCV to make predictions on whether a customer will just view an offer or if he is going to view and complete it.

## <a name="Description"></a> File Description
Starbucks_Capstone_notebook.ipynb - Jupyter Notebook that contains the analysis of the Starbucks capstone challenge.

## <a name="License"></a>Licensing, Authors, Acknowledgements
Must give credit to Starbucks for the data. I used the help of the stackoverflow community, the pandas and scikit-learn documentation.

## <a name="Summary"></a>Summary
Here are the key findings of my analysis:
* There's a consistent grow of Starbucks members year-over-year since 2013.
* There're more male members included in this data set than female members. Most of the members are in their 50's and 60's.
* BOGO offers have a higher viewing rate than discount offers, but discount offers have a higher completion rate than BOGO offers.
* Female members have a 10% to 25% higher completion raten than male members consistently across all offer types.
* In this scenario, the GradientBoostingClassifier is superior to the RandomForestClassifier when it comes to predicting if a member just views an offer or views and completes and offer.

To get a more detailed summary of my analysis, please read my medium post [here!](https://antonio-f-bauer.medium.com/starbucks-capstone-project-666057305ac8)
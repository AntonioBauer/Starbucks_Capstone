
# Starbucks Capstone Challenge
![](https://cdn.shortpixel.ai/client/q_lossy,ret_img,w_924/https://wichitaonthecheap.com/lotc-cms/wp-content/uploads/Starbucks-Happy-Hour-2.jpg)

## Table of Contents
1. [Project Motivation](#Project)
2. [File Description](#Description)
3. [Licensing, Authors, Acknowledgements](#License)
4. [Summary](#Summary)

## <a name="Project"></a>Project Motivation
This data set provided by Starbucks, contains simulated data that mimics customer behavior on their rewards mobile app. Once every few days, Starbucks sends out an offer to users of the mobile app. An offer can be merely an advertisement for a drink or an actual offer such as a discount or BOGO (buy one get one free). The goal of this project is to analyze how well certain customer groups respond to certain offer types by combining the three provided data sets. In order to achieve this goal, I had to clean and combine the three provided data sets first and then explore the data by visualizing it. Then the data was modeled, to be able to determine if an offer was viewed and then completed by am member. At the end, I used a GradientBoostingClassifier in combination with GridSearchCV to make predictions on whether a customer will just view an offer or if he is going to view and complete it.

## <a name="Description"></a> File Description
The portfolio data set has 6 columns and 10 rows, that describe the specifics of the 10 offers.

* portfolio.json - containing offer ids and meta data about each offer (duration, type, etc.)
* profile.json - demographic data for each customer
* transcript.json - records for transactions, offers received, offers viewed, and offers completed

### portfolio.json
* id (string) - offer id
* offer_type (string) - type of offer ie BOGO, discount, informational
* difficulty (int) - minimum required spend to complete an offer
* reward (int) - reward given for completing an offer
* duration (int) - time for offer to be open, in days
* channels (list of strings)

### profile.json
The profile data set consists of 5 columns and 17,000 rows, that describe the socio-demographics of the Starbucks members and the duration of their membership.

* age (int) - age of the customer
* became_member_on (int) - date when customer created an app account
* gender (str) - gender of the customer (note some entries contain 'O' for other rather than M or F)
* id (str) - customer id
* income (float) - customer's income

### transcript.json
The transcript data set contains 4 columns and 306,534 rows. This data set contains all transactions in regards to purchases and offers.

* event (str) - record description (ie transaction, offer received, offer viewed, etc.)
* person (str) - customer id
* time (int) - time in hours since start of test. The data begins at time t=0
* value - (dict of strings) - either an offer id or transaction amount depending on the record

## <a name="License"></a>Licensing, Authors, Acknowledgements
Must give credit to Starbucks for the data. I used the help of the stackoverflow community, the pandas and scikit-learn documentation.

## <a name="Summary"></a>Summary
Please find a summary of my findings on my medium post [here!](https://antonio-f-bauer.medium.com/starbucks-capstone-project-666057305ac8)
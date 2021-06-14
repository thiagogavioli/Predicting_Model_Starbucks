# Predicting Model for Starbucks offers (Udacity Data Science Capstone Project)

![](https://github.com/thiagogavioli/Predicting_Model_Starbucks/blob/main/starbuck.jpg)

## Table of contents
1. [Description](#Description)
2. [Installation](#Installation)
3. [File Descriptions](#File_Descriptions)
4. [Results](#Results)
5. [Licensing, Authors, Acknowledgements](#Licensing-Authors-Acknowledgements)

## Description

This is a a Capstone Project and it is part of Udacity's Data Science Nanodegree.

Data set of this project contains simulated data that mimics customer behavior on the Starbucks rewards mobile app. Once every few days, Starbucks sends out an offer to users 
of the mobile app. An offer can be merely an advertisement for a drink or an actual offer such as a discount or BOGO (buy one get one free). Some users might not 
receive any offer during certain weeks. Not all users receive the same offer, and that is the challenge to solve with this data set.

The task is to combine transaction, demographic and offer data to determine which demographic groups respond best to which offer type. This data set is a simplified 
version of the real Starbucks app because the underlying simulator only has one product whereas Starbucks actually sells dozens of products.

The analysis and solution explained in the notebook aims to use mathematical and statistical methods alongwith machine learning technics to find users more likely to 
buy Starbucks product, since they receive an offer. It relates to users on the Starbucks rewards mobile app, and I went over transaction, demographic and offer datasets 
provided by the company to accomplish this task. I am going to use exploratory data analysis to understand the data and get some insights, in addition to use Adaboost 
algorithm to create a machine learning model to predict if a costumer will convert or not, since Starbucks offers any of its promotion or information.


## Installation

**The dependencies are listed below:**

- jupyter 1.0.0
- numpy 1.17.4
- pandas 1.0.0
- matplotlib 3.1.1
- scikit-learn 0.22.1

## File_Descriptions

The data is contained in three files:

- portfolio.json - containing offer ids and meta data about each offer (duration, type, etc.)
- profile.json - demographic data for each customer
- transcript.json - records for transactions, offers received, offers viewed, and offers completed

Here is the schema and explanation of each variable in the files:

**portfolio.json**
- id (string) - offer id
- offer_type (string) - type of offer ie BOGO, discount, informational
- difficulty (int) - minimum required spend to complete an offer
- reward (int) - reward given for completing an offer
- duration (int) - time for offer to be open, in days
- channels (list of strings)

**profile.json**
- age (int) - age of the customer 
- became_member_on (int) - date when customer created an app account
- gender (str) - gender of the customer (note some entries contain 'O' for other rather than M or F)
- id (str) - customer id
- income (float) - customer's income

**transcript.json**
- event (str) - record description (ie transaction, offer received, offer viewed, etc.)
- person (str) - customer id
- time (int) - time in hours since start of test. The data begins at time t=0
- value - (dict of strings) - either an offer id or transaction amount depending on the record

## Results

The results are described in the following [blog post.](https://thiagogavioli.medium.com/improving-marketing-campaigns-to-starbucks-using-machine-learning-b57b2c0ddc1f)

## Licensing_Authors_Acknowledgements

Must give credit to Starbucks for the data used. The code can be used as any person demands.

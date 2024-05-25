# Alphabet Soup Foundation  deep-learning

## Overview 
The nonprofit foundation Alphabet Soup wants a tool that can help it select the applicants for funding with the best chance of success in their ventures. With my knowledge of machine learning and neural networks, I’ll use the features in the provided dataset to create a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup.

From Alphabet Soup’s business team, I have received a [CSV](https://static.bc-edx.com/data/dl-1-2/m21/lms/starter/charity_data.csv) containing more than 34,000 organizations that have received funding from Alphabet Soup over the years.

## Results

#### Data Preprocessing
![Screenshot 2024-05-24 234551](https://github.com/Seif-Ma/deep-learning-challenge/assets/152819459/86c1d3a9-d61f-428b-881b-7abe8e0dfa1b)

* The target variable for this model is the `IT_SUCCESSFUL` column, which indicate if the money was used effectively or not.
* The futures variables for the moedel include the following columns:
    *  `NAME` — Identification column
    *  `APPLICATION_TYPE` — Alphabet Soup application type
    *  `AFFILIATION` — Affiliated sector of industry
    *  `CLASSIFICATION` — Government organization classification
    *  `USE_CASE` — Use case for funding
    *  `ORGANIZATION` — Organization type
    *  `STATUS` — Active status
    *  `INCOME_AMT` — Income classification
    *  `SPECIAL_CONSIDERATIONS` — Special considerations for application
    *  `ASK_AMT` — Funding amount requested


* The variable that should be removed from the input data because it's neither target nor feature:  
    *  In the starter, I removed `EIN` and `NAME`, but I didn't reach my target.
    *  In thee optimization phase, I dropped just `EIN`, and that did lead to a better outcome.
 
![Screenshot 2024-05-25 000637](https://github.com/Seif-Ma/deep-learning-challenge/assets/152819459/065ef846-39e3-4feb-baa6-c03b62770e2c)

#### Compiling, Training, and Evaluating the Model

















## Summary


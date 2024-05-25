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

In the "Starter_Code" 


![Screenshot 2024-05-25 005855](https://github.com/Seif-Ma/deep-learning-challenge/assets/152819459/55cfba01-62d0-4284-b196-4cf4f914e7a1)


![Screenshot 2024-05-25 005949](https://github.com/Seif-Ma/deep-learning-challenge/assets/152819459/c0382fe4-a767-4623-8c44-5176ac3c1af0)



* To increase the model performance, I used `Karas_tuner` to auto optimize it:



![Screenshot 2024-05-25 002130](https://github.com/Seif-Ma/deep-learning-challenge/assets/152819459/88ebfb6b-a444-4884-9cfb-92aa472813cc)



![Screenshot 2024-05-25 002149](https://github.com/Seif-Ma/deep-learning-challenge/assets/152819459/15e18dd6-8fc0-42cd-b726-769be6440ade)



* The best model have the following hyperparameters: 

![Screenshot 2024-05-25 002343](https://github.com/Seif-Ma/deep-learning-challenge/assets/152819459/93f516d3-8165-45a6-b8aa-37012113447c)

* Then I applied those hyperparameters in the [AlphabetSoupCharity_Optimization](https://github.com/Seif-Ma/deep-learning-challenge/blob/main/AlphabetSoupCharity_Optimization.ipynb) file

![Screenshot 2024-05-25 011115](https://github.com/Seif-Ma/deep-learning-challenge/assets/152819459/c93b18f1-267e-4593-b81c-90f1c0923201)
![Screenshot 2024-05-25 011136](https://github.com/Seif-Ma/deep-learning-challenge/assets/152819459/981a2947-a8f5-4af0-ad07-b1bb7ae52612)

* That model have a 77.35% accuracy

![Screenshot 2024-05-25 011359](https://github.com/Seif-Ma/deep-learning-challenge/assets/152819459/579fec4b-af4a-4290-a95a-a627d049e6e1)

## Summary


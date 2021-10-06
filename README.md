# CreditRisk
Data Analysis on Loan Default through Lending Club data

## Motivation
Almost everyone goes through a loan of some kind, whether it is for a car or a house, in their entire life and they amount to a great fortune for banks. Interests are centainly where the profits are, but defaults are where the risk is, and so it is of particular interest to dig deeper into what factors affect loan defaults to help financial institutions understand and regulate loans in the financial market. The dataset is from the Lending Club at Kaggle at https://www.kaggle.com/wordsforthewise/lending-club.

## Files
[EDA](EDA.ipynb): Exploratory data analysis on the dataset with plots using seaborn and matplotlib.

[Model](Model.ipynb): Builds a baseline model and many larger models, performs model selection through Cumulative Accuracy Profiles and Area Under the Curve, investigates the tradeoff betweeen interpretability and predictability of a model, and conducts analysis to gain insights on the important factors of loan defaults.

### Key Takeaways and Notes
* Picked up accuracy ratio and cumulative accuracy profile
* Model consistent with credit grades assigned by lending club
* Investigated interpretability and predictability between simple and complicated models
* Analyzed the subgroup performance of models
* Random forest performs 10% better than logistic regression so we should take on the random forest if we were in industry because 10% of total loans is a large number, and logistic regression can still help us with analysis given the feature importance from the random forest as well
* Concluded that interest rate, the number of terms, and debt-to-income ratios are the most important factors in credit risk

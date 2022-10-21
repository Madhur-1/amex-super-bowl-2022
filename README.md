# amex-super-bowl-2022
AMEX Super Bowl 2022

Team Nexus
-------------------------------------------------------
https://unstop.com/competition/the-american-express-campus-super-bowl-american-express-433057

The American Express Campus Super Bowl is an analytics and data science-based competition for campus students. It's a platform to showcase your talent and compete with the best minds across India.

Our Decision Science & Strategy teams across Risk, Fraud, and Marketing are the backbone of all data-driven decisions across the customer life cycle at American Express. From targeting the right customer to underwriting to customer management every decision is powered by cutting-edge analytics & data science. Our best-in-class credit risk models and line assignment strategies have enabled us to maintain the industry’s best (lowest) credit loss numbers.

In this year’s competition, we are looking for innovative minds, who can better the results for our risk prediction models and line assignment strategies!

Note: Pls look at the Problem Statement.pdf file for a more detailed introduction.
-------------------------------------------------------

## Folder Description

### Data
Contains all thw data used for training the different models.
### Helpers
Contains random bit of cached data helpful for EDA and Modelling.
### Preds
Contains predicted probabilites by different models, mainly used for the Ensemble part.
### Submissions
Contains submission files.

## Verstack Library
Verstack was used for LGBM tuning and Missing value imputation. Look at https://github.com/DanilZherebtsov/verstack for more info.

# Flow

## EDA
Look at files with EDA in name. We start with looking for patterns in the data.

## Imputation
We try Mean-Median Imputation, Mean-Mean with Groupby imputation, , Sklearn Iterative Imputer and LGBM imputer for Abhishek Thakur's video https://www.youtube.com/watch?v=EYySNJU8qR0&ab_channel=AbhishekThakur on Handling missing values. Look for files with Imputation.

We finally go forward with Iterative Imputation.

## Feature Generation
Look at Feature Generation file for details.

## Modelling
Look at the files with Modelling for different models.

We finally use Random Forest, Neural Network, Logistic Regression, LGBM and XGBoost for ensembling. We also try Quadratic Discrimant Analysis.

We use Hyperopt for hyperparameter tuning. https://www.youtube.com/watch?v=5nYqK-HaoKY&t=3063s&ab_channel=AbhishekThakur

## Ensemble
We use the above mentioned 5 models and do Weighted averaging and Weighted Rank averaging. We also try Stacking.

https://www.youtube.com/watch?v=TuIgtitqJho&t=2371s&ab_channel=AbhishekThakur


TIP: Look at the Ideas to try.txt file for more exciting ideas.

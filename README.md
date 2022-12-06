# Coding exercise
The purpose of the following exercise is to assess your python skills, how you 
deal with timeseries data and be basis for discussion during the interview.

##  Tasks
### Task 1: python quiz
Please complete the notebook `python_quiz.ipynb` by solving the quick exercises contained there. Max time should be 1 hour.

### Task 2: modelling
#### Data
This repository contains two pickle files, `features.pkl` and `target.pkl`. 

`features.pkl` is a time-indexed Pandas dataframe with three columns, `0`, `1`, and `2`. The values 
represent the forecasted production from three forecast vendors for a portfolio of Ørsted windfarms. 
The units are MWh for the 30-minute window given by the index.
`target.pkl` contains the actual production from the portfolio for the same time range.
Both pickles contain pandas dataframes. The pandas version used for creation is specified in the requirements file.

#### The task
Your task is to create a Python class with an `sklearn`-style API (at least `fit`, `predict`, and 
`score` methods should be implemented) to predict the actual production based on the forecasted 
productions from the three vendors.

There is no limitation in terms of modeling techniques, feature engineering/cleaning, or extra data 
you may want to include. If you do include extra data, please add this to the submission.
Likewise, please add a `requirements.txt` file for any packages that are needed to run your code.

If the model takes more than a couple of minutes to train on a normal laptop, then please add a
method in the class to load a pre-trained model (e.g. by pickling it) and include the pickled
model in the submission.

We will evaluate:
- Code quality and any unit tests of your code you may wish to add.
- Feature engineering and model creation

You will be asked to talk about and go through your solution which you can do just by going through
your source code or in the form of a Jupyter notebook if that helps you present (we will look at
source code either way).
Please do not use more than two hours for this exercise. We suggest that you start by creating the model class and utilizing 
the simplest possible baseline model, and then take whatever time is left to incrementally improve the model. 
Whatever you do not manage to do, please make a note of and we'll have a discussion about it at the interview.

### Additional questions

Please also be ready to talk about/discuss the following

**Domain**
- If you had been able to ask questions about the domain, would that have helped you? What
 questions would you have asked?

**Technical**
- Argue why you chose the model you did, and why you did not choose something else?
- What would be a good baseline prediction? Why?
- Argue why you scored the model how you did.
- If you had had more time, what would you have done?

## Delivery
Please reply to the email, from which you got the link to this repo, with a link to a GitHub or
 GitLab repo containing your code, and please cc: `edsim@orsted.com`.

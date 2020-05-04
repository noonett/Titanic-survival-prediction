## What is Titanic?
	About a century ago, a great cruise was under constructing. After few years, it was ready to sail. Millions of people considered it the dream ship and the apex of ocean technology. Thousands of people were lucky enough to get one ticket on board. 4 days later, it sank. It is Titanic. The worst maritime disaster ever.
---
## What we want to do?
	By unlocking the inner association of these information, it is possible to find out what factors could make a passenger to survive from an ocean disaster. And build a classification model to predict if a passenger giving certain information can survive on Titanic.
---
## What about datas?
	It contains information of every passenger including name, sex, age, survived or not and so on.
* Dataset source: Kaggle
* Data dimension: 891 rows, 12 columns
---
## How to do it?
Step 1: Define variable ‘Survived’ as the target variable.

Step 2: Data treatment. By this step, it is expected to eliminate factor which is not correlated or less correlated to the target variable and null data in valuable column will be filled in fair way. Dummy encoding for nominal data, data split for train/test set will be implemented. 

Step 3: Model selection. The target variable is in Boolean type. Classification model such as Decision tree, Random forest and Logistic regression will be implemented. Naive Bayes method will be set up as baseline test. GridSearchCV will be implemented on each model to find the best parameter pair of each model in this data set. The best score and parameter pair of each model will be recorded.

Step 4: Ensemble model will be implemented; it consists of all classification models above. We will use ‘soft’ voting mode. The weight of each model will be adjusted by F1-score they hold. Also, accuracy and F1-score of ensemble model will be recorded.

Step 5: Conduct ROC and AUC of baseline model and the best model we got. McNemar's test on the best model and the baseline.

## Outcome:
Kaggle score: 0.785
Analysis report.
---
## Remarks:
5310assignment2.ipynb: code.
5310Assignment2.pdf: report.
assignment_presentation.pptx: slides.
test.csv: test data.
titanic.csv: training data.

# HR-Analytics-Classification

HR analytics is revolutionising the way human resources departments operate, leading to higher efficiency and better results overall. Human resources has been using analytics for years. However, the collection, processing and analysis of data has been largely manual, and given the nature of human resources dynamics and HR KPIs, the approach has been constraining HR. Therefore, it is surprising that HR departments woke up to the utility of machine learning so late in the game. Here is an opportunity to try predictive analytics in identifying the employees most likely to get promoted.

## Dataset
The dataset used is the HR Analytics Classification (https://www.kaggle.com/bhrt97/hr-analytics-classification) from Kaggle. This dataset has features:
- employee_id: Unique ID for each employee
- department: which department the employee belongs to (Ex: Sales & Marketing, Operations, etc)
- region: which place the person belongs to
- education: Education qualification (Ex: Bachelor's)
- gender: Male or Female
- recruitment_channel: How was he recruited (Ex: sourcing, other)
- no_of_trainings: Range from 1 to 9
- age
- previous_year_rating: Score from 1 to 5
- length_of_service
- KPIs_met: Key performance indicators 
- awards_won: either 1 or 0 (Yes or No)
- avg_training_score

Finally we must predict if the person must be promoted or no (Binary classification)

## Models used:
I have tested a total of 4 models on this dataset (Logistic Regression, Decision Trees, Random Forest, Naive Bayes)
### 1. Logistic Regression:
Logistic regression is a supervised learning classification algorithm used to predict the probability of a target variable. It has a similar concept of linear regression but we add a sigmoid function to it and make the graph like elongated S which helps in better predicting and modelling as now the data does not necessarily have to be linear it can be in other forms too. The most common logistic regression models a binary outcome; something that can take two values such as true/false, yes/no, and so on, and that is what we wanted here.

### 2. Decision Trees:
Decision Trees (DTs) are a non-parametric supervised learning method used for classification and regression. The goal is to create a model that predicts the value of a target variable by learning simple decision rules inferred from the data features. A tree can be seen as a piecewise constant approximation. On each step or node of a decision tree, used for classification, we try to form a condition on the features to separate all the labels or classes contained in the dataset to the fullest purity.

### 3. Random Forest:
Random forests or random decision forests are an ensemble learning method for classification, regression and other tasks that operates by constructing a multitude of decision trees at training time. For classification tasks, the output of the random forest is the class selected by most trees. This is basically like a collection of a lot of decision trees all working together on the same data (Many trees hence the name forest) and thus result in better result.

### 4. Naive Bayes:
In statistics, naive Bayes classifiers are a family of simple "probabilistic classifiers" based on applying Bayes' theorem with strong independence assumptions between the features. They are among the simplest Bayesian network models, but coupled with kernel density estimation, they can achieve higher accuracy levels.

## Future Work
We can try to perform  some more feature engineering to the dataset and some better way to oversampling the data as is_promoted has very few entries present (Directly using SMOTE analysis didn't perform well when I tried it for this dataset)

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

## Future Work
We can try to perfom some more feature engineering to the dataset and some better way to oversampling the data as is_promoted has very few entries present (Directly using SMOTE analysis didn't perform well when I tired it for this dataset)

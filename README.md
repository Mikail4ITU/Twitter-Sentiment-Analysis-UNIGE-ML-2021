# Twitter-Sentiment-Analysis-UNIGE-ML-2021

<img src="img/Geneva_School_of_Economics_and_Management.png"/>






In this project we worked on text data which was taken from social media platform Twitter. The train data has 1280000 tweets with 7 columns. The test data includes 320000 tweets and 6 columns. The only difference from train data is test data does not include the emotion column about corresponding tweet.

After completing all the steps in content of notebook we reached the following results.

We used two main classification algorithms which are Logistic Regression and LinearSVC.
Tfidf vectorizer used with n_range=(1,2).
The highest accuracy we got from test set provided was 0.8253 from LinearSVC(C=0.3) and 0.8209 LogisticRegression(C=0.9, max_iter=1000, penalty='l1', solver='liblinear')algorithm.However the text column we used was from the original training set without cleaning but with expanded date column features.
After using the cleaned_text column with expanded date column features from traindfcleaned we got accuracy 0.8126 from LinearSVC and 0.8118 from Logisitic Regression.
We used 5-Fold cross validation for tuning C hyperparameter.
We used dummified expanded date columns as predictor variables.
When we compare the results from training data(train-test split results) and kaggle submission we saw that the results were close. Therefore, before each submission we assessed the performance of the each algorithm.

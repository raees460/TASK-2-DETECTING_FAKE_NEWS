Task-2-Detecting-fake-news
For this endeavor, our goal is to identify fabricated news articles using Python alongside TfidfVectorizer and the PassiveAggressiveClassifier. Our approach involves training a model on a dataset of news articles, categorizing each piece as either genuine or fraudulent based on its content.

Dataset: The dataset employed consists of a CSV file containing 7796 entries across 4 columns: News: A unique identifier for each news article. Title: The headline of each news article. Text: The full text content of each news article. Label: The classification of the news article, either "real" or "fake".

Text Preprocessing: We performed preprocessing tasks such as removing stop words, punctuation, and other extraneous characters from the text data.

Feature Extraction: Utilizing TfidfVectorizer, we transformed the textual data into a TF-IDF feature matrix.

Model Training: We initialized a PassiveAggressiveClassifier and trained it using the TF-IDF matrix along with the corresponding labels.

Model Evaluation: To assess the model's performance, we computed its accuracy score and examined the confusion matrix.

Results: The model achieved an impressive accuracy score of 93.05%. Analysis of the confusion matrix revealed that the model accurately identified 161 fake news articles and 595 real news articles. However, it misclassified 21 fake news articles as real and 28 real news articles as fake.

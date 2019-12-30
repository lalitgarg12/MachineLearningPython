# Spam Detection
![images.png](images/spamintro.png)
## Basic Approach
When we choose to approach spam filtering from a machine learning perspective, we view the problem as a classification problem. That is, we aim to classify an email as spam or not spam (ham) depending on its features. In our case, the features are the count of each word in the email. 

## Pre Processing
After preliminary pre-processing (removing HTML tags and headers from the email in the data set), we take the following steps:
1. __Tokenize__ - We create "tokens" from each word in the email by removing punctuation.
2. __Remove meaningless words__ -  The text in red squares are stop-words, which should be removed. Stop-words do not provide meaningful information to the classifier, and they increase dimensionality of feature matrix. In addition to many stop-words, we removed words over 12 characters and words less than three characters.
3. __Stem__ -  The text in blue circle is converted to its "stem". Similar words are converted to its stem in order to form a better feature matrix. This allows words with similar meanings to be treated the same. For example, history, histories, historic will be considered same word in the feature matrix. Each stem is placed into our "bag of words", which is just a list of every stem used in the dataset. 
4. __Create feature matrix__ - After creating the "bag of words" from all of the stems, we create a feature matrix. The feature matrix is created such that the entry in row i and column j is the number of times that token j occurs in email i. 

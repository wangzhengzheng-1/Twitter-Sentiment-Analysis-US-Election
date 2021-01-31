# Twitter-Sentiment-Analysis-US-Election-2020
### Background:
Sentiment Analysis is a branch of Natural Language Processing (NLP) that allows us to determine algorithmically whether a statement or document is “positive” or “negative”. Sentiment analysis is a technology of increasing importance in the modern society as it allows individuals and organizations to detect trends in public opinion by analyzing social media content. Keeping abreast of socio-political developments is especially important during periods of policy shifts such as election years, when both electoral candidates and companies can benefit from sentiment analysis by making appropriate changes to their campaigning and business strategies respectively. The purpose of this assignment is to compute the sentiment of text information - in our case, tweets posted recently on US Presidential Elections 2020 - and answer the research question: “What can public opinion on Twitter tell us about the US political landscape in 2020?” The goal is to essentially use sentiment analysis on Twitter data to get insight into the 2020 American Elections. Central to sentiment analysis are techniques first developed in text mining. Some of those techniques require a large collection of classified text data often divided into two types of data, a training data set and a testing data set. The training data set is further divided into data used solely for the purpose of building the model and data used for validating the model. The process of building a model is iterative, with the model being successively refined until an acceptable performance is achieved. The model is then used on the testing data in order to calculate its performance characteristics.
### 1. Data cleaning : 
The tweets, as given, are not in a form amenable to analysis – there is too much ‘noise’. Therefore, the first step is to “clean” the data. Design a procedure that prepares the Twitter data for analysis by satisfying the requirements below. \n
o All html tags and attributes (i.e., /<[^>]+>/) are removed. \n
o Html character codes (i.e., &...;) are replaced with an ASCII equivalent.
o All URLs are removed.
o All characters in the text are in lowercase.
o All stop words are removed. Be clear in what you consider as a stop word.
o If a tweet is empty after pre-processing, it should be preserved as such.

### 2. Exploratory analysis :
o Design a simple procedure that determines the political party (Republican Party, Democratic Party and Others) of a given tweet and apply this procedure to all the tweets in the 2020 US elections dataset. A suggestion would be to look at relevant words and hashtags in the tweets that identify to certain political parties or candidates. What can you say about the distribution of the political affiliations of the tweets?
o Present a graphical figure (e.g. chart, graph, histogram, boxplot, word cloud, etc) that visualizes some aspect of the generic tweets in sentiment_analysis.csv and another figure for the 2020 US election tweets. All graphs and plots should be readable and have all axes that are appropriately labelled. 

### 3. Model preparation :
Split the generic tweets randomly into training data (70%) and test data (30%). Prepare the data to try multiple classification algorithms (logistic regression, k-NN, Naive Bayes, SVM, decision trees, ensembles (RF, XGBoost)), where each tweet is considered a single observation/example. In these models, the target variable is the sentiment value, which is either positive or negative. Try two different types of features, Bag of Words (word frequency) and TF-IDF. 

### 4. Model implementation and tuning :
Train models on the training data and apply the model to the test data to obtain an accuracy value. Perform hyperparameter tuning and cross-validation, if necessary.
Evaluate the same model with best performance on the 2020 US elections data. How well do your predictions match the sentiment labelled in the 2020 US elections data?
Choose the model that has the best performance and visualize sentiment prediction results and the true sentiment for each of the two parties/candidates. Discuss whether NLP analytics based on tweets is useful for political parties during election campaigns.
Split the negative 2020 US elections tweets into training data (70%) and test data (30%). Use true sentiment labels in the 2020 US elections data instead of your predictions from the previous part. Choose three algorithms from classification 
algorithms (logistic regression, k-NN, Naive Bayes, SVM, decision trees, ensembles (RF, XGBoost)), train multi-class classification models to predict the reason for the negative tweets. Tune the hyperparameters and chose the model with best score to test your 
prediction reason for negative sentiment tweets. There are 5 different negative reasons labelled in the dataset.

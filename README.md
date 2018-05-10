# NewsRecommendationTwitter
Github for Justin Tse and Cindy Xu's final project.

I have created an online app to run the entire news recommendation system. The app can be accessed at this link
https://justintse.shinyapps.io/newsrectwitter/

NOTE: SINCE GITHUB IS PUBLIC I HAVE BLOCKED OUT MY TWITTER AND NYT API KEYS.
To run the programs Twitter and NYT API keys are needed. I have blocked out my own keys but you can store your own keys in the following variables:
Twitter API: consumer_key, consumer_secret, access_token, access_secret
NYT API: NYTIMES_KEY

If you would like to run the News Recommendation GUI/APP locally instead of on the RShiny server, you need to provide your own keys. I would recommend running newsRecommendationGUI_FastVersion.R because it loads in a pre-trained model rather than training the model. I do not provide the dataset in this Github so you would need access to it if you want to run newsRecommendationGUI.R 

Files: 

newsRecomendationGUI_FastVersion.R - Fast version of the news recommendation GUI. It loads a pre saved bag of words model so there is no training necessary. 

bowModel_Apr9_2018.RData - Saved version of the bag of words model from data gathered in April. 

bagOfWords.R - Code for the Bag of Words Model, Also contains code to get training and test error.

DataCollection.R - Code to pull raw twitter data using Twitter API.

DataCompilation.R - Code to compile/process the data from different topics into a single file. 

NewsRecomendationGUI.R - Contains RShiny code that produces a GUI to recommend news articles to twitter users.

newsRecomender.R - Code to use a model and recommend news articles to a specific user.

Visualization.R - Code to produce visualizations. 

try.ipynb- Code for nueural network model

Try some new model- Code for MultinomialNB, LogisticRegression, LinearSVM and RandomForest.


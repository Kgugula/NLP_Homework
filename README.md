## NLP_Homework ##

For this homework assignment we performed NLP analysis on two cryptocurrencies: Bitcoin and Ethereum. The tools used in this assignment included: sentiment analysis, word clouds and tokenization, named entity recognition, and NGrams and frequeny analysis. 

# Sentiment Analysis #

    After importing relevant libraries and initializing my API key, I pulled data from the web related to the two cryptocurrencies (using NewsAPI). I then created some functions to iterate through the requested data (it was in JSON format), and transform it into a pandas DataFrame. From there I used Vader Sentiment Analyzer to evaluate the tone of the news articles. Both crpyocurrencies had similiar sentiment analysis results - which is to be expected since they are biggest players in the crpyto world, and a lot of people (myself included) use their names to generalize about all other cryptocurrencies (e.g. like Kleenax used to describe all 'facial tissues'). It retrospect it would have been interesting to pull data from a Twitter and evaluate sentiment scores, see if there is much divergence between the official news reports and the internet's 'public square.' 

# Natural Language Processing #

    For this part of the homework I tokenized the words in the coin's respective articles DF's. Had some trouble here but found a work around with a function I built (see 'organize and tokenize').

    Then we set ngrams = 2 and took a look at common word pairings. There wasn't that many repitions.

    Then I found 10 most common words in each DF. The words that did repeat didn't provide to much value. I had to go back and rerun the kernel adding new stopwords each time because at first it was only no value-add words. My guess if that if you were doing this type of analysis enough your stop words list would be # huge # --> and maybe you would have different ones for different types of reports (e.g. Bank of Canada vs. Earnings). Very cool to see the tokenized word lists appended on the dataframes. You can immediately see the value they provide.

    Lastly built word clouds. They were pretty cool to render but, again, the words weren't to striking or informative. Nonetheless a nice visual. 

# Named Entity Recognition #

    In the last section of the homework I used the Spacy and Displacy libraries to render a document with all of the named entities highlighted. This part was pretty cool and I immediately saw the value when you can just skim over a piece of text quickly and git the jist of it. You would be able to 

# Concluding Thoughts #

    Natural Language Processing, at least for me, feels more defined as a stand alone FinTech domain. It is hard to fatham all of the potential applications for this in the future. My mind immediately goes into analyzing the sentiment of particular corpus' almost instantaneously. And imagine if it was possible to mix in some 'machine learning' component whereby the computer gets better and better at predicting sentiments/decisions of individuals JUST before they actually say the word. 

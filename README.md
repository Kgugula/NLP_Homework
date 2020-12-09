# NLP_Homework

For this homework assignment we performed NLP analysis on cryptocurrencies, namely, Bitcoin and Ethereum. The tools used in this assignment included: sentiment analysis, words clouds and tokenization, and named entity recognition

# Sentiment Analysis #

    After importing relevant libraries and setting up a NewsAPI key, I pulled data from the web related to the two cryptocurrencies. I then created some function to clean the requested data (it was in JSON format), and transform it into a pandas DataFrame. From there I used Vader Sentiment Analyzer to evaluate the aggregate tone of the news articles. Based on this analysis. Both crpyocurrencies had similiar sentiment analysis results - which is to be expected since they are biggest players in the crpyto world, and a lot of people (myself included) use their names to generalize about all other cryptocurrencies (e.g. like Kleenax used to describe all 'facial tissues'). Answers to the related questions are in the notebook.

# Natural Language Processing #

    For this part of the homework I tokenized the words in the coin's respective articles DF's to put them into a more digestable format for the computer. Had some trouble here but found a work around with a function I built (see 'organize and tokenize'). 

    Then we set ngrams = 2 and took a look at common word pairings. There wasn't that many repitions.

    Then I found 10 most common words in each DF. The words that did repeat didn't provide to much value. I had to go back and rerun the kernel adding new stopwords each time because at first it was only no value-add words. 

    Lastly built word clouds. They were pretty cool to render but, again, the words weren't to striking or informative. 

# Named Entity Recognition #

    In the last section of the homework I used the Spacy and Displacy libraries to render a document with all of the named entities highlighted. This part was pretty cool and I immediately saw the value when you can just skim over a piece of text quickly and git the jist of it, because all the important stuff was highlighted. 
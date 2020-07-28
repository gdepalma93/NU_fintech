# NLP Problem Set

## Background
--- 
There's been a lot of hype in the news lately about cryptocurrency, so you want to take stock, so to speak, of the latest news headlines regarding Bitcoin and Ethereum to get a better feel for the current public sentiment around each coin.

In this Problem Set, you will apply natural language processing to understand the sentiment in the latest news articles featuring Bitcoin and Ethereum. You will also apply fundamental NLP techniques to better understand the other factors involved with the coin prices such as common words and phrases and organizations and entities mentioned in the articles.

### Files
    - problem_set
    - starter_files
        - crypto sentiment notebook
    - solutions
        - crypto sentiment solution
    - guides
        - student guide
        - nlp environment set up
        - nueral network cheatsheet
 
### Libraries
    - ML Libraries
        - nltk
        - wordcloud
        - spacy
    - Data Science Libraries
        - pandas
        - os
### SDK's
    - newsapi
        
### ML Techniques
    - Sentiment Analysis
    - Natural Language Processing
        - Tokenization
        - n-grams
        - frequency analysis
        - word clouds
    - named entity recognition
    
### Outputs
   - Sentiment Scores
   - Tokenized Language
   - N-gram analyis
   - frequency analysis
   - word clouds
   - Named Entity Visualization 
--- 

## Problem Set
    1. Sentiment Analysis
        1.1) Use the newsapi to pull the latest news articles for Bitcoin and Ethereum and create a DataFrame of sentiment scores for each coin.
            1.1.a) Which coin had the highest mean positive score?
            1.1.b) Which coin had the highest negative score?
            1.1.c) Which coin had the highest positive score?
    2. Natural Lanaguage Processing
        2.1) Tokenization
            2.1.a) Lowercase each word
            2.1.b) remove punctuation
            2.1.c) remove stop words
        2.2) Analysis
            2.2.a) Use NLTK to produce the ngrams for N=2
            2.2.b) List the top 10 words for each coin.
        2.3) Generate word clouds for each coin to summarize the news for each coin.
            
    3. Named Entity Recognition
        3.1) Build a named entity recognition model for both coins and visualize the tags using SpaCy
        


        
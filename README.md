# Unit_12_Assignment

## 1. Sentiment Analysis (Ln 1-9)
In this section we: 
* Complete the initial imports, read our api key environment variable, create a newsapi client,  and fetch the Bitcoin and Ethereum news articles (Ln 1-5). 
* Create the Bitcoin and Ethereum Sentiment Scores Dataframes ('dfs') by using for loops, and passing in the variables we created for our news articles (Ln 6-7). 
* Describe the Bitcoin and Ethereum Sentiment and conclude that Ethereum had the highest *mean positive*, *compound* and *maximum positive scores*. We also conclude that Ethereum and Bitcoin have identical maximum *negative scores*(Ln 8-9). 

## 2. Natural Language Processing (Ln 10-25)
In this section we:
* Import the nltk and re packages from python, together with tools that will help us to tokenize, lemmatize, identify stopwords and remove unwanted punctuation(Ln 10). 
* Instantiate our lemmatizer, create a list of stopwords, and define our tokenizer function (Ln 11-12). 
* Using the tokenizer function above, create new tokenizer columns for Bitcoin and Ethereum (Ln 13-14).
* Import Counter and ngrams from collections and nltk, respectively (Ln 15). 
* Create variable for Bitcoin tokens column , combine tokens from list of lists into one large list, and display btc_tokens_list and  generate the Bitcoin N-grams (using the  btc_tokens_list where N=2 (Ln 16-17). 
*  Similarly,  we repeat kernels 16-17 but for Ethereum (Ln 18-19). 
* Create a function  'token_count()',  which will generate the top 10 words for either coin, and use the token_count to generate the top 10 words for Bitcoin (by passing in btc_tokens_list that we created above). Similarly we obtain the top 10 words for Ethereum (Ln 20-22). 
* Import the wordcloud and matplotlib libraries and dependencies to generate our wordcloud visualizations (Ln 23). 
* Generate the Bitcoin and Ethereum wordclouds, by passing btc_tokens_list and eth_tokens_list (described earlier) into our 'join()' function (Ln 24-25). 
*

## 3. Named Entity Recognition (Ln 26-36)
In this section we:
* Import the spaCy library and its displaCy visualizer,  download the language model for SpaCy, and load the spaCy model (Ln 26-28). 
* Concatenate all of the Bitcoin text together, by defining a new variable 'btc_text' and using the '.str.cat()' function instead of a cumbersome for loop (Ln 29).  
* Run the NER processor on all  the text by passing in btc_text,  render our visualization of named entities for Bitcoin, and list all entities in our Bitcoin text (Ln 30-32). 
* Similarly to kernels 29-32, we concatenate all our Ethereum text together, run the NER processor on our variable eth_text, render our visualization of named entities for Ethereum, and list all entities in our Ethereum text (Ln 33-36). 

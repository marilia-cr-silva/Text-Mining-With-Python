# Sentiment Analysis and Text Mining with Python

## [SCC5920] Project (2020.2) - Text mining - Institute of Mathematics and Computer Science - University of São Paulo

Files and folders:

* **[code] Mining_Twitter_with_Python.ipynb:** this file contains the Jupyter Notebook concerning the Tweepy library with API. It requires a Twitter developer account, so that you get the keys and tokens. Depending on your account - standard, premium, enterprise - you are allowed to mine more tweets and a longer time horizon. My account is a standard one. Thus, I can only mine 100 tweets at time with the function API.search. It requires iterating, and post-processing steps in order to ensure that there are not duplicated tweets. The .txt file contains four lines - consumer_key, consumer_secret, access_token and access_token_secret - API authentication.

* **[code] Pre_processing_Tweets_with_Python.ipynb:** after excluding duplicated tweets (based on tweet ID and/or full_text), this notebook can process spreadsheets according to transformers or simple language processing models such as Bag-of-Words. The file loaded a stemmer in Portuguese. Thus, it is recommended changing the language. In addition, depending on your preferences, all you need is to remove the stemmer, since there is an intrinsic semantic loss. This code, in spite of it's scalable, has a template. It is mandatory that the header of the first column is "sentence" and the last column "target", which is the classification attributed to the tweet - there are intermediate columns as well if the tweet is split into several sentences. The header of other columns can have any name.

* **[folder] Pre-processing-inputs:** this folder has library files and spreadsheets before pre-processing.

* **[folder] Pre-process-outputs:** the files were created at Colab, so that they can be processed with Transformers (such as BERT) and Bag-of-Words.

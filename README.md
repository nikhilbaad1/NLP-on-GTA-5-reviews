# NLP-on-GTA-5-reviews
This project aimed at predicting the sentiment of the review as good, bad, or average of the GTA V game. NLP techniques are used to form TFIDF vectors and  Bag Of Words. These vectors are then used with the Machine Learning classification algorithm to predict the sentiment.


SCRAPING DATA: The data is scraped from Google and amazon reviews. The amazon site now blocks bots, scrapers, and crawlers. To overcome this, the Selenium driver is used. Scraping.ipynb file scraps the data.

TRANSLATION OF TEXT: Translation of text is done differently for Google and amazon as amazon data needed some further pre-processing. For detecting the text language langdetect is used. To translate the text translators library is used to request google translator. Google reviews didn’t have any other languages but amazon reviews were in many languages.

EMOJI TO TEXT: To convert emoji to text emoji library is used.

TRANSLATION OF SLANG/ SHORTENED WORDS: To translate this the first the slang words dictionary is scraped. Slan_words.ipynb file scrapes the dictionary and stores it in json format as ShortenedText.json. 

![image](https://user-images.githubusercontent.com/47523576/236007320-f052d84b-6ddb-4121-875b-267dd8026f79.png)

MACHINE LEARNING:
Vector	                                  Algorithm	       Train Acc.	Test Acc.
Uni-gram TFIDF	                          Random Forest	   85.80	    85.805
Uni-gram TFIDF top 10 features	          Random Forest	   86.44	    86.92
Uni-gram TFIDF	                          Naïve Bayes		   55.01
Uni-gram TFIDF	                          Kernal SVM	     83.63	
Uni-gram top 2500 features	              NLTK Naïve Bayes 85.63	    82.35
Bag of Words	                            Random Forest	   86.12	    85.08
Bi Grams TFIDF	                          Random Forest	   84.03	    84.76
Top 20000 Bigrams and 2000 Unigrams TFIDF	Random Forest	   85.01	    84.92


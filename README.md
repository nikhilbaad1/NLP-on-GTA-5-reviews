# NLP-on-GTA-5-reviews
This project aimed at predicting the sentiment of the review as good, bad, or average of the GTA V game. NLP techniques are used to form TFIDF vectors and  Bag Of Words. These vectors are then used with the Machine Learning classification algorithm to predict the sentiment.


SCRAPING DATA: The data is scraped from Google and amazon reviews. The amazon site now blocks bots, scrapers, and crawlers. To overcome this, the Selenium driver is used. Scraping.ipynb file scraps the data.

TRANSLATION OF TEXT: Translation of text is done differently for Google and amazon as amazon data needed some further pre-processing. For detecting the text language langdetect is used. To translate the text translators library is used to request google translator. Google reviews didn’t have any other languages but amazon reviews were in many languages.

EDA:

Word Cloud

![image](https://user-images.githubusercontent.com/47523576/236011286-21bc3d86-de74-4f32-a3f4-edcd36e3f7d4.png)

20 most common words

![image](https://user-images.githubusercontent.com/47523576/236011351-25f54d71-eb1c-4150-aa7e-93ff57d30b8c.png)



EMOJI TO TEXT: To convert emoji to text emoji library is used.

![image](https://user-images.githubusercontent.com/47523576/236010751-04d2e495-779d-4d12-89c3-11c3c001b159.png)


TRANSLATION OF SLANG/ SHORTENED WORDS: To translate this the first the slang words dictionary is scraped. Slan_words.ipynb file scrapes the dictionary and stores it in json format as ShortenedText.json. 

![image](https://user-images.githubusercontent.com/47523576/236007320-f052d84b-6ddb-4121-875b-267dd8026f79.png)


MACHINE LEARNING:

<img width="280" alt="image" src="https://user-images.githubusercontent.com/47523576/236010961-19ac236d-e66a-4452-bb6b-0cb0c1209577.png">

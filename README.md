🛒 **Twitter Analysis of Online Dutch Supermarkets in times of COVID-19**
==============================
![image_project_supermarket_covid](https://github.com/dpbac/twitter_analysis_online_grocery_NL/blob/master/images/image_project_supermarket_covid.JPG)

This project aims to analyze the sentiment related to three of the biggest (online) supermarkets in the Netherlands and their customers in the period of the corona crisis. The data used were collected using Twitter API and consisted of Tweet from users’ (i.e. supermarkets) timeline and Tweets obtained from queries.
Data was collected using Twitter API, then some cleaning and manipulation was made to have the data in suitable format for analysis. Some research was performed to find out which NLPs tools were more suitable for the NLP analysis since more than 93% of the Tweets are in Dutch and most of the tools are used for English. EDA and sentiment analysis were performed showing the impact of COVID-19 also when considering (online) grocery shopping. 

Project Organization
------------
    │
    ├── README.md          <- The top-level README for developers using this project.
    │
    ├── data
    │   ├── external       <- Data from third party sources.
    │   ├── interim        <- Intermediate data that has been transformed.
    │   ├── processed      <- The final, canonical data sets for modeling.
    │   ├── raw            <- The original, immutable data dump.
    │   └── tweets         <- Retrieved tweets.
    │
    ├── notebooks          <- Jupyter notebooks. Naming convention is a number (for ordering),
    │   │                      the creator's initials, and a short `-` delimited description, e.g.
    │   │                     `1.0-jqp-initial-data-exploration`.
    │   └── twitter_credentials.py	   <- Contains Twitter credentials
    │
    ├── references         <- Data dictionaries, manuals, and all other explanatory materials.
    │
    │
    └── requirements.txt   <- The requirements file for reproducing the analysis environment, e.g.
	                         generated with `pip freeze > requirements.txt`


--------

# Some tools used:

* [Python-twitter](https://python-twitter.readthedocs.io/en/latest/index.html)
* [TextBlob](https://textblob.readthedocs.io/en/dev/)
* [textblob-nl](https://github.com/gvisniuc/textblob-nl)
* [langdetect](https://pypi.org/project/langdetect/)
* [LangID](https://pypi.org/project/langid/1.1dev/)
* [Textcat from nltk](https://www.nltk.org/_modules/nltk/classify/textcat.html)  
* [Spacy](https://spacy.io/)
* [Seaborn](https://seaborn.pydata.org/index.html)

# Notebooks


**[01-collecting_and_saving_tweets.ipynb](https://github.com/dpbac/twitter_analysis_online_grocery_NL/blob/master/notebooks/01-collecting_and_saving_tweets.ipynb):** Collect data using methods of the Twitter API. Some pre-processing and saving data in .csv.
**Notebook 02:** Concatenate most recent and older data from AH’s user timeline in order to increase the period covered. Investigate and use different language detector in order to full fill information of language of Tweets that were missing. Process Tweets obtained from queries.
**Notebook 03:** Perform feature selection, concatenate data of all three supermarkets considering the chosen, calculate sentiment of Tweets.
**Notebook 04:** Perform EDA and sentiment analysis on Tweet data covering the period of `30th March, 2020 till 24th June, 2020`.

This period does not cover all period considering the 1st corona case in The Netherlands (February 27th) but as seen in the following 
graph still covers an important period of the crisis.

![Compare period of corona crisis and period covered by research.](https://github.com/dpbac/twitter_analysis_online_grocery_NL/blob/master/images/period_covered.png)

# Install/Technical requirements

* You'll need Twitter API credentials to run this project. In [01-collecting_and_saving_tweets.ipynb](https://github.com/dpbac/twitter_analysis_online_grocery_NL/blob/master/notebooks/01-collecting_and_saving_tweets.ipynb) replace `private_twitter_credentials.py` by `twitter_credentials.py`. `twitter_credentials.py` must contain your [Twitter 
credentials](https://developer.twitter.com/en/docs/basics/authentication/oauth-1-0a/obtaining-user-access-tokens).

* conda version: 4.8.3
* Install requirements using `pip install -r requirements.txt`.
  * Make sure you use Python 3 (I used 3.6.7).
  * You may want to use a virtual environment for this.

<p><small>Project based on the <a target="_blank" href="https://drivendata.github.io/cookiecutter-data-science/">cookiecutter data science project template</a>. #cookiecutterdatascience</small></p>

Project_twitter_analysis_online_grocery_NL
==============================

The goal of this project is to perform a sentiment analysis in relation to online grocery shopping in the Netherlands considering the period starting with the 1st case of corona virus or as close as possible of this. For this we will use Twitter messages.

Project Organization
------------
    │
    ├── README.md          <- The top-level README for developers using this project.
    │
    ├── data
    │   ├── external       <- Data from third party sources.
    │   ├── interim        <- Intermediate data that has been transformed.
    │   ├── processed      <- The final, canonical data sets for modeling.
    │   └── raw            <- The original, immutable data dump.
    │
    ├── notebooks          <- Jupyter notebooks. Naming convention is a number (for ordering),
    │                         the creator's initials, and a short `-` delimited description, e.g.
    │                         `1.0-jqp-initial-data-exploration`.
    │
    ├── references         <- Data dictionaries, manuals, and all other explanatory materials.
    │
    │
    ├── requirements.txt   <- The requirements file for reproducing the analysis environment, e.g.
    │                         generated with `pip freeze > requirements.txt`
    │
    └── twitter_credentials.py	   <- Contains Twitter credentials


--------

# USAGE

In [notebook]() replace `private_twitter_credentials.py` by `twitter_credentials.py`. `twitter_credentials.py` must contain your [Twitter 
credentials](https://developer.twitter.com/en/docs/basics/authentication/oauth-1-0a/obtaining-user-access-tokens).

<p><small>Project based on the <a target="_blank" href="https://drivendata.github.io/cookiecutter-data-science/">cookiecutter data science project template</a>. #cookiecutterdatascience</small></p>

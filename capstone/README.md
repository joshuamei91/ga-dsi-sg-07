# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) DSI 7 Capstone Project: Fake News Classification

This project uses the Liar Liar Pants on Fire [dataset](https://arxiv.org/abs/1705.00648) to explore classification of news statements. The aim is to train different classifiers to categorize the statements as false, half true or true.

## Business Case

Disinformation is becoming more prevalent with greater impact in today’s world . This is due to the proliferation of technology that allows people to disseminate and access information from all sorts of sources in real time. This allows fake news to spread more easily and rapidly; it could incite violence, cloud people’s opinions, manipulate elections and impact the operations of media platforms.

Therefore, companies such as Facebook, news agencies and government agencies have a vested interest in detecting such disinformation early and handling them. However, the staggering volume of information generated everyday makes it unpractical to sift through and ascertain the veracity of every statement. Therefore, this project aims to automate the classification of the veracity of statements. This could help companies or governments to optimise the effort in investigating fake news.

## Dataset

The dataset contains training, validation and test sets with labeled statements from Politifact and meta-data related to the statements. There are 6 labels: pants on fire, false, barely true, half true, mostly true and true. I did not think that such granularity was necessary, hence I grouped the statements into 3 classes instead: false, half true and true. The meta-data includes information such as the speaker, context, party affiliation of the speaker etc. 

## Notebook workflow

1. Data cleaning and exploratory data analysis
2. Feature engineering (eg. proportion of Part of Speech, parse tree depth)
3. Modelling with Bag of Words (BOW)
4. Modelling with BOW + engineered features + meta-data features
5. Investigate model coefficients
6. Analysis and limitations

---

## Resources 

These are some of the resources that greatly helped me in the project:

### Towards Data Science articles by Dipanjan (DJ) Sarkar

- [Traditional Methods for Text Data](https://towardsdatascience.com/understanding-feature-engineering-part-3-traditional-methods-for-text-data-f6f7d70acd41)

- [A hands-on intuitive approach to Deep Learning Methods for Text Data — Word2Vec, GloVe and FastText](https://towardsdatascience.com/understanding-feature-engineering-part-4-deep-learning-methods-for-text-data-96c44370bbfa)

- [A Practitioner's Guide to Natural Language Processing (Part I) — Processing & Understanding Text](https://towardsdatascience.com/a-practitioners-guide-to-natural-language-processing-part-i-processing-understanding-text-9f4abfd13e72)

### Google's Machine Learning Guide to Text Classification

- https://developers.google.com/machine-learning/guides/text-classification/

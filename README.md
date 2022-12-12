# Stock-Market-Prediction-using-NLP-over-Reddit-Data-
# Dataset Explanation:
The data set is used from kaggle and the link of the data is
https://www.kaggle.com/aaron7sun/stocknews.
Two types of data provided in this dataset:
1. News data: Browsed through Reddit World News Channel's historic news headlines.
They are classified with the revised votes of the users, and just a single date is taken in
the top 25 headlines.
2. Stock Data: "Proving the idea" is based on the (DJIA).
## Tf-idf and implementation of Simple classification:
The phrases were played into words by using the RegexpTokenizer nltk, starting from the daily
headlines. There is also an application of lemmatization. This is the responsibility of the
following CustomTokenizer.
The TfidfVectorizer converts the raw headlines into a TF-IDF feature matrix with the
CustomTokenizer.
● English stop words are deleted, words are transformed from upper case to lowercase.
● The ngram_range are taken into account
● Min_df Ignore words with strictly higher document frequency than the particular
threshold the training dataset used for vectorization.
![image](https://user-images.githubusercontent.com/61366086/207012522-a6215530-a315-4693-97c7-3502ff7453a3.png)
## Some Common Headlines of the data
![image](https://user-images.githubusercontent.com/61366086/207012648-962bd570-3bf1-41cc-892b-5c5828b6d3c0.png)
## Implementation of Keras Sequential model:
There is a sequence and functionality of two approaches to construct Keras models.
For most situations, the sequential API enables you to construct layer-by-layer models. The fact
that you can not construct models which share layers or have many inputs or outputs is restricted.
The functional API also gives you the possibility to construct much more flexible models,
because you can simply define models whose layers are more connected than only the past and
the next levels. You can actually link layers to any other layer (literally). This makes it possible
to create complicated networks, such as Siamese and residual networks.
 ## Model Loss:
Loss is the fine for a wrong forecast. That is to say, loss is a number which shows how terrible
the forecast of the model was with one sample. If the forecast of the model is perfect, the loss
must be zero, otherwise the loss shall be larger. The objective of the model training is to identify
![image](https://user-images.githubusercontent.com/61366086/207012875-3f32686b-f011-4c1f-af9e-1fd3e313fc71.png)

# Some Data Preprocessing used in this method:
## Removing Stop words:
Stops words are the words which usually used in any language and in the case of English
language there are number of stop words i.e is, are, am, the etc. and these words are not
beneficial for training the data in NLP so we can remove these words and the benefit of
removing these words is that we have data in more cleaned form.
## Tokenization
Tokenization is an important technique in NLP which converts the text into tokens like there are
5 words in a sentence and after tokenization it will be five tokens and it will call word
tokenization.
5.1.3 Stemming and Lemmatization:
Stemming and lemmatization are procedures used to evaluate the meaning behind a word in
search engines and catboats. Stemming employs the word's stem and the context in which the
term is employed in the lemmatization. More explanations and examples will be provided later.
We want relevant results to be found not just for the precise term that we put into the search
field, but also for any alternative versions of the words we use when performing a search.
## Word embedding
An embedding word is a learning representation of a text with a comparable meaning in words.
This method is one of the main advances of in-depth study on the hard challenges in the
processing of natural languages.


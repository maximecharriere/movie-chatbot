# movie-chatbot

### JupyterNotebook:
This NoteBook can totaly be run on **GoogleColab**, try it!   --> <a href="https://colab.research.google.com/github/maximecharriere/movie-chatbot/blob/master/MoviesClassifier/movie-classifier.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>

### Usefull Links:
- [The Definitive Guide to Natural Language Processing (NLP)](https://monkeylearn.com/blog/definitive-guide-natural-language-processing/)
- [Text Classification](https://monkeylearn.com/text-classification/)
- [Short Text Classification](https://monkeylearn.com/short-text-classification/)
- [Text Classification Using Naive Bayes](https://monkeylearn.com/text-classification-naive-bayes/)
- [Text Classification Using Support Vector Machines (SVM)](https://monkeylearn.com/text-classification-support-vector-machines-svm/)
- [Word embeddings: how to transform text into numbers](https://monkeylearn.com/blog/word-embeddings-transform-text-numbers/)
- [The Beginner’s Guide to Text Vectorization](https://monkeylearn.com/blog/beginners-guide-text-vectorization/)
- [Sentiment Analysis](https://monkeylearn.com/sentiment-analysis/)
- [Deep Learning for NLP](https://medium.com/dair-ai/deep-learning-for-nlp-an-overview-of-recent-trends-d0d8f40a776d)
- [Google text classification Guide](https://developers.google.com/machine-learning/guides/text-classification/)
- [Genre classification based on wiki movies plots](https://www.kaggle.com/aminejallouli/genre-classification-based-on-wiki-movies-plots/notebook#3.-Classifiers-Training)


### Vocabulary list
- Creat the vocabulary list with all words stem found in the training set


### Algoritm
#### Text processing
Can be done with:
* [spaCy](https://spacy.io/)
* [NLTK](https://www.nltk.org/)
 1. Lower case
 1. Standardizing numbers (ex. '12' -> 'number')
 1. Transform question mark ('?' -> 'questionmark')
 1. Word Stemming (ex. 'discount', 'discounts', 'discounted', 'discounting' -> 'discount')
 1. Removal of non-usefull characters/words (ex. stop words, ponctuation)
#### Features
Word to vectors:
* [GloVe](https://nlp.stanford.edu/projects/glove/)
* [word2vec](https://pathmind.com/wiki/word2vec)
 6. For the input text, fill a list of the size of the vocabulary list, with the score of each word.
    The following scoring method can be use for n-gram:
    * Binary, i.e. the word is present or not in the text
    * Count, i.e. the number of time the word appear in the text
    * Frequency, i.e. Count/Total number of words in the text
    * TF-IDF (Term Frequency – Inverse Document Frequency), i.e. the score increase with the word frequency, but a penality is given if this word is widely used in the training set (like 'for', 'a', 'the'). The scores have the effect of highlighting words that are distinct (contain useful information) in a given text.
 6. If the dataset is big and the sentence are small, we can use word embeddings.
 
 Temps Colab 25min, Temps local 22min
#### Classification
 8. SVM is machine learing algorithm, MLP is a deep learning algorithm
    * [Multinomial Naive Bayes (MNB)](https://monkeylearn.com/text-classification-naive-bayes/)
    * [Support Vector Machines (SVM)](https://monkeylearn.com/text-classification-support-vector-machines-svm/)
    * [Multilayer perceptron (MLP)](https://en.wikipedia.org/wiki/Multilayer_perceptron)


### Notes
- Il faut avoir le même nombre de features pour n'importe quel text
- La structure et l'ordre des mots est perdu

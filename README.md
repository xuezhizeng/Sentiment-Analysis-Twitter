# Twitter Sentiment Analysis

##NLTK basics

**Lemmatizer** :
`WordNetLemmatizer().lemmatize("better",pos='v')`
->good

**Similarity**:
`
w1 = wordnet.synset("ship.n.01")
w2 = wordnet.synset("boat.n.01")
print w1.wup_similarity(w2)
`
->90%

**Classifier**:
`
all_words = []
for w in movie_reviews.words():
    all_words.append(w.lower())
all_words = nltk.FreqDist(all_words)
print all_words.most_common(15)
print all_words["stupid"]
`

##Approach
Using 
* Stochastic Gradient Descent
* Multinomial Naive Bayes
* Bernoulli Naive Bayes
* LogisticRegression
* Support Vector
* LinearSVC
* NuSVC

Files positive1.txt and negative1.txt are used to train the data.  
_positive1.txt_ includes positive reviews of a movie.    
_negative1.txt_ includes negative reviews of a movie.

Twitter API is used to grab current trending tweets in real-time and use the trained classifiers to mark them as a _'positive'_ or a _'negative'_ sentiment. A graph is hence plotted.

**NOT COMPLETED YET**

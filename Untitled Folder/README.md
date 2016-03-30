# NLTK

Lemmatizer :
WordNetLemmatizer().lemmatize("better",pos='v')
->good

Similarity:
w1 = wordnet.synset("ship.n.01")
w2 = wordnet.synset("boat.n.01")
print w1.wup_similarity(w2)
->90%

Classifier:
all_words = []
for w in movie_reviews.words():
    all_words.append(w.lower())

all_words = nltk.FreqDist(all_words)

print all_words.most_common(15)
print all_words["stupid"]

    
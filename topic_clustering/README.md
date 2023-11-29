
# Topic clustering using LDA

Topic clustering is unsupervised task since we use unlabeled data. The aim of topic clustering is to categorize corpus of text into homogenized clusters (just like what we have in clustering tasks).

In this project, I use a sample of 2000 news texts as the data source. Then, I apply various text cleaning and preprocessing techniques to make the corpus ready for various clustering methods. Afterwards, I use kmeans and LDA to cluster the text and compare the results. 

You can find the dataset [here](https://github.com/sajadahmadia/NLP/blob/main/topic_clustering/raw_data.csv)





## Procces
I did the whole process by mostly using the gensim and nltk libraries (as well as numpy and pandas).

1. Text preprocessing, in fact, getting the juice of words by applying various techniques like lammatization, selecting specific part of speech tags, .... 
2. Tokenizing sentences into words
3. Using LDA model to get the clusters
4. Checking the clusters by eye
## Lessons Learned

 I didn't try to to clean up the unexpected results that might happen when doing topic clustering, because it is the reality of our job. Each investigation provides some ideas for further and better models, and we come up with a newer model, and again and again ....

Totally, I found only foure meaningful clusters and then changed the names of the clusters to a more human-friendly version.



## Future Actions
Future Actions
For future actions, I use the word lemmatizer from the spacy library instead of the nltk library and see the results, Since I see both "said" and "say" in the first cluster as high frequent words. The word lemmatizer from the nltk doesn't convert past tense verbs like "said" to their present tenses(like "say").

I also might try kmeans and other clustering methods and compare results.
## Author

- [@sajadahmadia](https://github.com/sajadahmadia)


## 🛠 Skills
Python, NLP, NLTK, SPACY, GENSIM



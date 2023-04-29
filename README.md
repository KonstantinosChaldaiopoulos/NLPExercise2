# NLP exercise 2

In this exercise, we have completed a series of tasks related to word embeddings and traditional text classification using the pre-trained word embeddings, word2vec (word2vec-google-news-300) and GloVe (glove-wiki-gigaword-300) included in gensim, and the AG News Topic Classification dataset with the scikit-learn library.

## Question 1 (Code File: Question1):
We analyzed word2vec and GloVe embeddings to find the closest words to given words, such as 'car', 'jaguar', 'Jaguar', and 'facebook', and compared the results to identify common words in the results from both embeddings. We also repeated this task with four words of our choice. Next, we found the 10 closest words to the word 'student' and provided lists of words that are not related to university students or primary, middle, or high school students. We then worked with analogies to find the closest words using both word2vec and GloVe embeddings and repeated the process with three analogies of our choice, commenting on the results.

## Question 2 (Code File: Question2):
We implemented various text classification approaches using the scikit-learn library, including Multinomial Naïve Bayes with tf-idf word uni-grams and character tri-grams representations, and Support Vector Machines (linear kernel, C=1) with tf-idf word uni-grams and character tri-grams representations. We reported the performance (accuracy on test set), dimensionality (number of different n-grams used), and time cost (in seconds) of these models in a table. Finally, we identified specific texts in the test set that all models misclassify, showed the contents of one such text, reported the number of such texts per category (World, Sports, Business, Sci/Tech), and identified the most common pair of correct category and wrong prediction for these texts.


## Question 3 (Code folder: Question3):
We have evaluated the performance of different RNN and LSTM models on the text classification task using the AG News Topic Classification dataset. The models include single-layer unidirectional RNN (1RNN), single-layer bidirectional RNN (1Bi-RNN), two-layer bidirectional RNN (2Bi-RNN), single-layer unidirectional LSTM (1LSTM), single-layer bidirectional LSTM (1Bi-LSTM), and two-layer bidirectional LSTM (2Bi-LSTM). We have referred to the tables in the Question1 and Question2 code files, which demonstrate the models' accuracy on the test set, their complexity (number of parameters), and their time cost (average seconds per epoch).

It should be noted that the one-directional RNN (1RNN) code was provided by the teacher.

We have analyzed how the model performance is affected by their complexity, how the time cost is affected by their complexity, and how much the use of two layers helps in improving the model's performance. We have also identified specific texts in the test set that all models misclassify, showed the contents of one such text, reported the number of such texts per category (World, Sports, Business, Sci/Tech), and identified the most common pair of correct category and wrong prediction for these texts.

Additionally, we have explored the effect of changing the MAX_WORDS parameter from 25 to 50 and compared the results with those from the previous part. We have examined how this change affects RNN and LSTM models in terms of performance and complexity.

Furthermore, we have modified the code to initialize the network embeddings with pre-trained embeddings (glove-6B-100d), reported the code changes, and repeated the analysis with MAX_WORDS=25. We have discussed the impact of using pre-trained embeddings on model performance and complexity.

We have also repeated the previous analysis but froze the GloVe embeddings during the training of the network. We have reported the code changes and discussed the resulting performance compared to the previous part.

Finally, we have adapted the code to work with the IMDB movie review dataset, which consists of 50k movie reviews classified into two categories (positive and negative). We have used 80% of the dataset as the training set and the remaining 20% as the test set. We have repeated the analysis for the IMDB dataset, following the same process as in sub-question a.

The detailed results and code implementation for these additional tasks can be found in the Question3 code folder.

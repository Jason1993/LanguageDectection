# Language Detection
## This is a Fellowship.ai Challenge

The training data set is from [European Parliament Proceedings Parallel Corpus](http://www.statmt.org/europarl/). And the [test data set](https://storage.googleapis.com/google-code-archive-downloads/v2/code.google.com/language-detection/europarl-test.zip) is from the link.

This is language detection program, I use the idea from the paper [N-Gram-Based Text Categorization](http://www.let.rug.nl/vannoord/TextCat/textcat.pdf).

Basically, in every language corpus, I store the top 50 most frequent uni-Grams, bi-Grams, and tri-Grams, and then for every unlabeled document, we calculate the distance from document to each language, and we pick the shortest distance language as the language of the document.

The main idea of this model is simple and it gets an acceptable accuracy as 95.15%.

To run this program on your own environment, you will need to modify the file path of training corpus, also the file path of test set need to be changed correctly.

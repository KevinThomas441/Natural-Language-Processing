# N-gram Language Models
In this project, we trained probabilistic language models to distinguish between words in different languages. Rather than looking up whole words in a dictionary, we built models of character sequences to make guesses about the language of unseen words. We use NLTK and the Universal Declaration of Human Rights corpus. We compare different languages from the Universal Declaration of Human Rights documents.

We built unigram, bigram, and trigram character models for the languages. For each word in the English test sets, we calculated the probability assigned to that string by English vs. French unigram models, English vs. French bigram models, and  English vs. French trigram  models. We used the test set to report accuracy of our models

## Required Libraries
<ul>
  <li>NLTK</li>
</ul>

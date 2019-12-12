# Text Classification and Analogy Tests
## Text Classification

<ul>
<li>We   needed   functions   to   assess   and   evaluate   the performance of our models. We implemented those first.
  
<li>Majority  Class  Baseline.  We   created majority  class baseline  to evaluate  our initial model  performance –which is  the  simplest baseline.  The  label  for  the  test  data  was the  majority  class  found  in training data.

<li>Review  Length  Baseline.  We created a  baseline  to evaluate  our  model  performance –which  takes  into  account  length  of  the review. For  this  baseline,  we  tried  setting  various  thresholds  of review  length  to classify  them  as positiveor  negative.  For  example,  all  reviews  >  50  words  in length were classified  as  positive.
  
<li>Implementing the Naïve Bayes classifier. We implemented Naive Bayes to classify the movie reviews based on TF-IDF vectors created using the corpus.
  
<li>Further we implemented Support Vector Machine Classifier to perform our classification task.
</ul>

## Vector Semantics
Similar  to  language models, embeddings    are    trained    directly    from    a    large  collection    of    natural language  text  without  being  tied  to  a  specific  NLP application   or subtask.   How   can   we   measure   the quality   of   learned embeddings? Some of the commonly accepted extrinsic evaluation methods are based on word similarity tasks, word analogies (e.g., “man is to woman as king is to queen) We explored an analogy task. The analogy prediction task is defined as follows. Given a pair of words <a, b> and a third word c,choose a fourth-word dso that the analogy <a is to b> as <c is to d> holds.
  
Analogy  Dataset: Mikolov’s  analogy  dataset includes  four  semantic  relationsand  four  syntactic relations.  In  the  test  files,  each  line  represents  one  analogy question, in the form of four words <a, b, c, d>.For example: “Bangkok Thailand Cairo Egypt”A  question  is  counted  as  correctly  answered  only  if  the  predicted  word  is  the same  as  the  given  word.  For  example,  given  the  first  three  words  “Bangkok Thailand Cairo”, the task is to predict “Egypt”. The full set of analogy questions can be found in the file word-test.v1.txt. 

The  groups  of  relations  are  delimited  by  lines  starting  with  a  colon  (:)  and  you should only work with these groups: capital-world, currency, city-in-state, family, gram1-adjective-to-adverb,  gram2-opposite,  gram3-comparative,  and  gram6-nationality-adjective. Word  Embeddings“Pretrained”  word  embeddings  are  word  embeddings  that are already constructed in advance of your NLP project (whether your project is a neural language model, a text classifier, or a class assignment). The advantage of  pretraining  is  that  it  simplifies  learning  your  model,  because  the  embedding parameters  are  fixed  in  advance.  The  disadvantage  is  that,  if  your  embeddings happen  to  be  bad  for  your  task,  you’re  stuck  with  them.

<ul>
<li>We ran  the  analogy  test on two sets  of  pretrained embeddings,  implement  the  analogy  prediction  method  and  compare  their  accuracies on  eight  analogy  tasks.
<li>One  known  problem  with  word  embeddings  is  that antonyms (words with meanings considered to be opposites) often have similar embeddings. We discuss  why  embeddings might have this tendency. 
<li>We designed two new types of analogy tests that are not part of  Mikolov’s  analogy  dataset.
</ul>

## Required Files
<ul>
  <li>https://ai.stanford.edu/~amaas/data/sentiment/</li>
  <li>http://www.fit.vutbr.cz/~imikolov/rnnlm/word-test.v1.txt</li>
</ul>

## Required Libraries
<ul>
  <li>NumPy</li>
  <li>Pandas</li>
  <li>Scikit Learn</li>
  <li>Gensim</li>
  </ul>

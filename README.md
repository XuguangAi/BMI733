# BMI733

## Overiew

In this project we investigate on "popularity" of questions on Reddit. We use number of comments to define "popularity" of questions. We pick 10 most active 
subreddits and choose the threshold for each subreddit such that the proportions of popular and unpopular posts are closest to fifty-fifty.  It is tabulated as
below: 

![](./dataset.png)

Note the threshold in the table is included in the unpopular posts. For example, in r/AskHistorians, the post with number of comments ≤ 2 is classified as unpopular and the post with number of comments ≥ 3 is classified as popular.

We classify each post as either popular or unpopular based on its threshold and gather 100,000 posts with labels 1 (popular) and 0 (unpopular). There are 10 topics in total and 10,000 posts from each topic. We divide 100,000 questions into 80,000 training examples and 20,000 testing examples. 20,000 testing examples are exactly the same for all 3 methods and we do not touch the testing dataset at all during the training.

## Methods

This is a binary classification task to predict popularity of questions. We use 3 methods to predict whether a post is popular or unpopular based on its title question: Convolutional Neural Network (CNN), Bidirectional Long Short-Term Memory (BiLSTM) which is a Recurrent Neural Network (RNN) architecture, and Bidirectional Encoder Representations from Transformers (BERT).

### CNN

It is in CNN&RNN

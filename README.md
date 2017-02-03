# Randomly-Generated-Tweets

Train a stochastic model to recognize patterns in speech drawn from any body of text and output randomly-generated sentences that mimic the sentence structure of whatever text the model was trained on. I used this program to create the tweets posted at @Random_Trump, a Twitter account that posts randomly-generated sentences in the same style as @realDonaldTrump's tweets. Please note that this program is <b>not</b> intended to make any kind of political point, I simply needed a popular Twitter account to train the model that powers this program. To see an example of this program in action, you can check out <a href="https://twitter.com/Random_Trump">@Random_Trump's Twitter page here.</a>

This program is built on top of two open-source platforms: <a href="http://twitter4j.org/en/index.html">Twitter4j</a>, a native Java wrapper for the Twitter API that significantly simplifies the calling interface; and <a href="https://rednoise.org/rita/">RiTa</a>, a software toolkit for computational literature. This program mainly functions as a command-line tool that can first create a Markov Chain with RiTa that has been trained on a Twitter user's Tweets (pulled programmatically from Twitter via Twitter4j), randomly generates a given number of sentences that mimic the sentence structure of the training set, and then posts the randomly-generated sentences back to a new Twitter account via Twitter4j. 


# Summary

Tweebank v2 is a collection of English tweets annotated in Universal Dependencies that can be exploited for the training of NLP systems to enhance their performance on social media texts.

# Introduction

Tweebank v2 is built on the original data of Tweebank v1 (840 unique tweets, 639/201 for training/test set), along with an additional 210 tweets sampled from the POS-tagged dataset of Gimpel et al. (2011) and 2,500 tweets sampled from the Twitter stream from February 2016 to July 2016.
The latter data source consists of 147.4M English tweets. In the same way as Kong et al. (2011),
reference unit is always the tweet in its entirety
-- which may thus consist of multiple sentences -- not the sentence alone.
Before annotation, we use simple regular expression to anonymize username and URL.

Our annotation process was conducted in two stages.
In the first stage, 18 researchers worked on the Tweebank v1
proportion and the additional 210 tweets and created the initial annotations in one day.
Before annotating, they were given a tutorial overview of the general UD
annotation conventions and our guidelines specifically for annotating tweets.
Both the guidelines and annotations
were further refined by the authors of this paper to increase
the coverage of our guidelines and solve inconsistencies between
different annotators during this exercise. In the second stage, a tokenizer, a POS tagger, and a
parser were trained on the annotated data from the first stage (1,050 tweets in total),
and used to automatically analyze the sampled 2,500 tweets.  Authors 
of this paper manually corrected the parsed data and finally achieved 3,550 labeled tweets.

# Corpus splitting

The treebank has been randomly split as follows:

* en-ud-tweet-train.conllu: 1,639 tweets (24,753 words)
* en-ud-tweet-dev.conllu: 710 tweets (11,742 words)
* en-ud-tweet-test.conllu: 1,201 tweets (19,112 words)


# References

* Yijia Liu, Yi Zhu, Wanxiang Che, Bing Qin, Nathan Schneider, and Noah A. Smith. 2018. [Parsing Tweets into Universal Dependencies](https://www.aclanthology.org/N18-1088/). In Proc. of NAACL.
* Lingpeng Kong, Nathan Schneider, Swabha Swayamdipta, Archna Bhatia, Chris Dyer, and Noah A. Smith. 2014. [A Dependency Parser for Tweets](https://www.aclanthology.org/D14-1108/). In Proc. of EMNLP.
* Kevin Gimpel, Nathan Schneider, Brendan O’Connor, Dipanjan Das, Daniel Mills, Jacob Eisenstein, Michael Heilman, Dani Yogatama, Jeffrey Flanigan, and Noah A. Smith. 2011. [Part-of-speech tagging for Twitter](http://www.aclanthology.org/P11-2008): Annotation, features, and experiments. In Proc. of ACL.

# Changelog

2018-04-15 v2.0

* initial release

# Metadata

```
Data available since: UD v2.1
License: CC BY-NC-SA 4.0
Includes text: yes
Genre: social
Lemmas: automatic
UPOS: automatic with corrections
Relations: automatic with corrections
Contributors: Liu, Yijia; Zhu, Yi; Schneider, Nathan; Smith, Noah A.
Contributing: elsewhere
Contact: oneplus.lau@gmail.com
```

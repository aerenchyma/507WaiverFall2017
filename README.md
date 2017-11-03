# 507WaiverFall2017
Waiver exam for University of Michigan SI 507. You must complete all 3 parts, and the code for each part must be checked in to github with the name specified for that part. Any other filenames will break our grading system and will be rejected.

## Part 1: Create a program to analyze the twitter timeline of a selected user.

FILENAME: part1.py

ARGUMENTS: the program takes two arguments--a twitter username and the number of tweets to analyze.

OUTPUT: the program outputs the following:
* the user name
* the number of tweets analyzed
* the five most frequent verbs that appear in the analyzed tweets
* the five most frequent nouns that appear in the analyzed tweets
* the five most frequent adjectives that appear in the analyzed tweets
* the number of _original_ tweets (i.e., not retweets)
* the number of times that the _original_ tweets in the analyzed set were favorited
* the number of times that the _original_ tweets in the analyzed set were retweeted by others

NOTES: 
* use tweepy for accessing the Twitter API
* Use NLTK for analyzing parts of speech. Use NLTK's default POS tagger and tagset (this will use the [UPenn treebank tagset](https://www.ling.upenn.edu/courses/Fall_2003/ling001/penn_treebank_pos.html))--you do NOT need to install any taggers or tagsets into NLTK.
* stop words: ignore any words that do not start with an alphabetic character `[a-zA-Z`], and also ignore 'http', 'https', and 'RT' (these show up a lot in Twitter)
* a "verb" is anything that is tagged VB*
* a "noun" is anything that is tagged NN*
* an "adjective" is anything that is tagged JJ*
* for the nouns, verbs, and adjectives, don't worry about the fact that there might be words that have the same frequency and will therefore be listed in random order. We'll account for this in our grading.

SAMPLE OUTPUT:

```bash
mwnewman$ python3 get_tweets.py umsi 50
USER: umsi
TWEETS ANALYZED: 50
VERBS: are(4) being(3) is(3) improve(2) Join(2) 
NOUNS: umsi(8) UMSI(8) students(5) Join(5) amp(5) 
ADJECTIVES more(5) umsi(4) doctoral(2) new(2) social(2) 
ORIGINAL TWEETS: 27
TIMES FAVORITED (ORIGINAL TWEETS ONLY): 69
TIMES RETWEETED (ORIGINAL TWEETS ONLY): 18
```

## Part 

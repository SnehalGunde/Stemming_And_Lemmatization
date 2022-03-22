# Stemming_And_Lemmatization

## What is Stemming?
 
We already know that a word has one root-base form but having different variations, for example, “play” is a root-base word and playing, played, plays are the different forms of a single word. So, these words get stripped out, they might get the incorrect meanings or some other sort of errors.   
 
The process of reducing inflection towards their root forms are called Stemming, this occurs in such a way that depicting a group of relatable words under the same stem, even if the root has no appropriate meaning. 
 
Moreover;
Stemming is a rule-based approach because it slices the inflected words from prefix or suffix as per the need using a set of commonly underused prefix and suffix, like “-ing”, “-ed”, “-es”, “-pre”, etc. It results in a word that is actually not a word.
There are mainly two errors that occur while performing Stemming, Over-stemming, and Under-stemming. Over-steaming occurs when two words are stemmed from the same root of different stems. Under-stemming occurs when two words are stemmed from the same root of not a different stems. Two types of stemmers are:
 
### Defining Porter Stemmer
 
Porter Stemmer uses suffix striping to produce stems. It does not follow the linguistic set of rules to produce stem for phases in different cases, due to this reason porter stemmer does not generate stems, i.e. actual English words. 
 
It applies algorithms and rules for producing stems. It also considers the rules to decide whether it is wise to strip the suffix or not. A computer program or subroutine that stems word may be called a stemming program, stemming algorithm, or stemmer.
 
### Defining Snowball Stemmer
 
Martin Porter, an inventor of the Snowball programming language, developed it to support other languages. It’s an advanced version of Porter Stemmer, also named as  Porter2 Stemmer. 
 
For example, if you print the word “badly” with the help of Snowball in English and Porter, we get different results. Consider the code context below;  
 
print(SnowballStemmer("English").stem("badly"))
Output: bad
 
Here, the word “badly” is stripped from the English language using Snowball Stemmer and get an output as “bad”. Now, snowball Stemmer is used for stripping the same word from the Porter language, we get the output as “badli”   
 
print(SnowballStemmer("porter").stem("badly"))
Output: badli
 
The above example clearly shows that the Snowball stemmer is better than Porter Stemmer.
 
## What is Lemmatization?
 
In simpler forms, a method that switches any kind of a word to its base root mode is called Lemmatization. 
 
In other words, Lemmatization is a method responsible for grouping different inflected forms of words into the root form, having the same meaning. It is similar to stemming, in turn, it gives the stripped word that has some dictionary meaning. The Morphological analysis would require the extraction of the correct lemma of each word. 
 
For example, Lemmatization clearly identifies the base form of ‘troubled’ to ‘trouble’’ denoting some meaning whereas, Stemming will cut out ‘ed’ part and convert it into ‘troubl’ which has the wrong meaning and spelling errors.
 
‘troubled’ -> Lemmatization -> ‘troubled’, and error
‘troubled’ -> Stemming -> ‘troubl’
 
 

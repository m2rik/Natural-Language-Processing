# Natural-Language-Processing
# Spam Detection



# Sentiment Analysis

## STEP 1 - Normalize
 -Lemitize the words
 -Then we need to remove STOP WORDS since it doesnt required much

## STEP 2 - BOW 
To convert data into features we need to first make a BAG OF WORDS
Since this is Sentimental Analysis problem we need to look for the words like NOT, NEVER. Since we are doing BOW, 
which will loose the text sequence, if the sentence contains Negation words then remove that word and append _NOT to other words
in that sentence.
Requires only UNIGRAM BOW. since it is sentimental analysis problem. 

For BOW score - we will take TFIDF , since domain is the same for all the data (medical domain). 
So there can be many medical words which will be throuthout the text like 'symptoms','Thyroid'
so TFIDF will give very low score to such a words. And Good score to the unique words which are present in each class

## STEP 3 - Smoothing
Just to avoid 0 multiplication we will do smoothing 

## STEP 4 - Modelling
Apply a Naive bayes model on BOW

## STEP 5 - Additional Steps
Finding emotions from 'AND' 
If there are some emotion base words that does not contain in Train set, but we can find out using AND method
E.g Service is Nice and XYZ. # here XYZ meight be positive


# Language Modelling

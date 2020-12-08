# Word_Prediction
Coursera Capstone Project -Word Prediction
Welcome to my next word prediction Capstone Project. This was a wonderful learning experience and a first step in doing a NLP Model processing. This would not be possible without the numerous reference articles posted in the capstone project forum, discussions from all students doing the course, NLP language model related videos , CRAN vignettes.


I have built this model opting to perform the "next word" prediction only using 2 grams due to the mere fact that memory is an issue when hosting this code in the shiny App server that has free 1GB quota only. 

The flow logic is as follows:
1. Take 10% of the blogs, news and twit( english only) text and read them into a corpus.
2. Perform all the possible cleanup and preprocessing on your data 
3. Build 2 gram to 4 gram model words and store them in RDS files 
4. Always when running your code from second time, make use of the RDS files to read in the data, as this is much faster than processing it every time
5. Remove profanity words
6. Build your prediction function to return the most probably next word whenever a user will type a word in the App,similar to Phone Keyboard.

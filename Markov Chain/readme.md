# Project 'Markov Chain'

---

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)

This project was made for the **'Artificial Intelligence'** course in my university.

There are two parts:
- an implementation of the **Markov Chain** with variable number of states
- using **NLTK Sentiment Analyzer** on a Shakesperian text

### Markov Chain 
A basic implementation of a class that trains on some text (in this case Romanian poetry) and then can generate sentences.
You have the option to set how many states do you want the Markov Chain to use.

### NLTK Sentiment Analyzer
We analyze a part of a Shakesperian text to get some date for every line.

This is an example:

    My reason, the physician to my purpose bred, That all the Muses filed.           - compound: 0.0, neg: 0.0, neu: 1.0, pos: 0.0,                                    
    Thus policy in love, to thee resort.                                             - compound: 0.6369, neg: 0.0, neu: 0.588, pos: 0.412,                             
    Against my love alone.                                                           - compound: 0.4939, neg: 0.244, neu: 0.244, pos: 0.512,  

Then we take a random word from each line and change it to the most similar word using **Word2Vec**.
The **blue** words means the word changed, the **red** ones means that Word2Vec could not find a similar word.

For the final part we calculate a **BLEU score**.
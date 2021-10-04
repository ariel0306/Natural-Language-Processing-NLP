# Natural Language Processing (NLP) Project


Project Topic
---
Stance prediction of fake news detection 

Project Goal
---
The task is to detect fake news by predicting the stance associated to every news article using the FNC dataset
https://github.com/FakeNewsChallenge/fnc-1 . The FNC dataset consists of 49,973 pairs of
headlines and article bodies. The body text is annotated by the following classes: agree,
disagree, discuss or be unrelated to the headline.
The model Input is expected to include a headline and a body text
The model is then designed to classify the stance of the body text relative to the claim
made in the headline into one of four categories:
- **Agrees**: The body text agrees with the headline
- **Disagrees**: The body text disagrees with the headline
- **Discusses**: The body text discusses the same topic as the headline, but does not take
a position
- **Unrelated**: The body text discusses a different topic than the headline
The data suffers from an imbalance problem where around 70% of the articles are
unrelated. 

Project Description
---
1) Apply two feature extraction techniques and discuss briefly how they work and their
advantages and disadvantages.  
a) Term Frequency-Inverse Document Frequency **(TF-IDF)**  
b) A dense word embedding **(Word2Vec)** 
2) Two-step Classification:   
a) Related/Unrelated classification:      
i) Use the features extracted from the step above to train a standard **Machine
Learning method** (e.g., SVM, Logistic Regression, Random Forest) and discuss its
performance on the testing set to classify whether the article body is related or
unrelated given the headline. 
- ii) Train one **Deep Learning model** of your choice (e.g., LSTM, RNN, CNN) using TFIDF (1.a) and dense word embedding (1.b). Explain and justify the architecture of
the deep learning model, the hyper-parameters used, and the loss function.
- iii) Analyse and compare the performance and training time results for both ML and
DL models.
- b) Agree/Disagree/Discuss classification:
Build a new deep learning model on top of the best performing model you
implemented in a), report its performance and discuss the results
- i) Based on the output of the model built in a), build a deep learning model of your
choice to classify related articles into the remaining three categories
(Agree/Disagree/Discuss).
- ii) Analyse the performance of your model and report the results
- c) Combine the two models in a) and b) to test your model end to end, report and
discuss the overall performance of your solution



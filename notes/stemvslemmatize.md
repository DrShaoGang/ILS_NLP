---
layout: page
title: Stemming VS Lemmatization 
nav_exclude: true
permalink: /notes/stemvslemmatize/
---

# Stemming VS Lemmatization 

It is easier to build a stemmer for a language than it is to build a lemmatizer for that language. Stemming tends to be faster because it performs only some string manipulation. A lemmatizer is slower because it must look up each word, and you might also need to calculate which part of speech a word is. 
While lemmatization is a more complex method and it usually works better than stemming to map a word to its stem form. 

Whether stemming or lemmatizing gives you the best results depends on the type of problem that you want to solve. You must also consider the tradeoffs that you might need to make in terms of performance versus accuracy.

In the example below, the lemmatized version has fewer tokens, and the words are and was are mapped to be. This mapping could improve the results of the model that you are training, depending on the problem that you are working on.

Original sentence <br>
"the children are playing outside. the weather was better yesterday."  <br>
Stemming => “the children are play outside. the weather was better yesterday” <br>
Lemmatization => “the child be play outside. the weather be good yesterday” <br>




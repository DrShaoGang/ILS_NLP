---
layout: page
title: Vectorizing Text
nav_exclude: true
permalink: /notes/textvectors/
---

# Vectorizing Text
Machines only understand numerical numbers. In this section, we will explore how to convert text data into a numerical representation.![image]

## Bog-of-Words (BOW)
Bag-of-words (BOW) converts text data into numbers. BOW does this conversion by creating a vocabulary from all the words in all the documents. It then calculates the occurrences. <br>
- BOW creates a vocabulary from the words in all documents.
- BOW Calculates the occurrences of words:
  - Binary (present or not) - Indicates whether the word is present or not present.
  - Word counts – Counts how many times the word appears in the text.
  - Frequencies – Provides a count of the words, normalized across the document.

|                              | a | cat | dog | is | it | my | not | old | wolf |
|---------------------------------------|---|---|---|---|---|---|---|---|---|
| “It is a dog.”                        | 1 | 0 | 1 | 1 | 1 | 0 | 0 | 0 | 0 |
| “my cat is old”                       | 0 | 1 | 0 | 1 | 0 | 1 | 0 | 1 | 0 |
| “It is not a dog, it is a wolf.”      | 1 | 0 | 1 | 1 | 1 | 0 | 1 | 0 | 1 |

 
  <br>
One challenge of BOW is how to handle new words that were not part of the original vocabulary. This issue is known as out-of-vocabulary (OOV), and you will come back to it later in this section.

  <br>

## Term Frequency (TF)
Term frequency (TF): Increases the weight for common words in a document. <br>
𝑡𝑓(𝑡𝑒𝑟𝑚, 𝑑𝑜𝑐)= (𝑛𝑢𝑚𝑏𝑒𝑟 𝑜𝑓 𝑡𝑖𝑚𝑒𝑠 𝑡ℎ𝑒 𝑡𝑒𝑟𝑚 𝑜𝑐𝑐𝑢𝑟𝑠 𝑖𝑛 𝑡ℎ𝑒 𝑑𝑜𝑐)/(𝑡𝑜𝑡𝑎𝑙 𝑛𝑢𝑚𝑏𝑒𝑟 𝑜𝑓 𝑡𝑒𝑟𝑚𝑠 𝑖𝑛 𝑡ℎ𝑒 𝑑𝑜𝑐)  <br>

|                              | a | cat | dog | is | it | my | not | old | wolf |
|---------------------------------------|---------|---------|---------|---------|---------|---------|---------|---------|---------|
| “It is a dog.”                        | 0.25    | 0       | 0.25    | 0.25    | 0.25    | 0       | 0       | 0       | 0       |
| “my cat is old”                       | 0       | 0.25    | 0       | 0.25    | 0       | 0.25    | 0       | 0.25    | 0       |
| “It is not a dog, it is a wolf.”      | 0.22    | 0       | 0.11    | 0.22    | 0.22    | 0       | 0.11    | 0       | 0.11    |

  <br>

## Inverse Document Frequency (IDF)
Inverse document frequency (IDF): Decreases the weights for commonly used words, and increases weights for rare words that are in the vocabulary. <br>
𝑖𝑑𝑓(𝑡𝑒𝑟𝑚)=log⁡(𝑛_𝑑𝑜𝑐𝑢𝑚𝑒𝑛𝑡𝑠/(𝑛_(𝑑𝑜𝑐𝑢𝑚𝑒𝑛𝑡𝑠 𝑐𝑜𝑛𝑡𝑎𝑖𝑛𝑖𝑛𝑔 𝑡ℎ𝑒 𝑡𝑒𝑟𝑚)+1))+1
<br>


| Term  | IDF Calculation             |
|-------|-----------------------------|
| a     | log(3/3) + 1 = 1             |
| cat   | log(3/2) + 1 = 1.18          |
| dog   | log(3/3) + 1 = 1             |
| is    | log(3/4) + 1 = 0.87          |
| it    | log(3/3) + 1 = 1             |
| my    | log(3/2) + 1 = 1.18          |
| not   | log(3/2) + 1 = 1.18          |
| old   | log(3/2) + 1 = 1.18          |
| wolf  | log(3/2) + 1 = 1.18          |
<br>


## TF-IDF
Term frequency-inverse document frequency (TF-IDF): Combines term frequency and inverse document frequency. <br>

𝑡𝑓_𝑖𝑑𝑓 (𝑡𝑒𝑟𝑚,𝑑𝑜𝑐)=𝑡𝑓(𝑡𝑒𝑟𝑚, 𝑑𝑜𝑐)∗𝑖𝑑𝑓(𝑡𝑒𝑟𝑚)  <br>

|                              | a | cat | dog | is | it | my | not | old | wolf |
|---------------------------------------|---------|---------|---------|---------|---------|---------|---------|---------|---------|
| “It is a dog.”                        | 0.25    | 0       | 0.25    | 0.22    | 0.25    | 0       | 0       | 0       | 0       |
| “my cat is old”                       | 0       | 0.3     | 0       | 0.22    | 0       | 0.3     | 0       | 0.3     | 0       |
| “It is not a dog, it is a wolf.”      | 0.22    | 0       | 0.11    | 0.19    | 0.22    | 0       | 0.13    | 0       | 0.13    |


 <br>

 







BOW
TF-IDF
N-gram
Word2Vec
Bert embeddings

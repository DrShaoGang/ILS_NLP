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












BOW
TF-IDF
N-gram
Word2Vec
Bert embeddings

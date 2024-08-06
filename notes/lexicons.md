---
layout: page
title: Sentiment Analysis Lexicons
nav_exclude: true
permalink: /notes/lexicons/
---



# Sentiment Analysis Lexicons

Sentiment analysis lexicons are essential tools in Natural Language Processing (NLP) for determining the sentiment expressed in text. These lexicons contain lists of words or phrases associated with various sentiment scores, which can be used to analyze the emotional tone of a given text. This document provides an overview of some widely used sentiment analysis lexicons and includes resources for further exploration.

## What Are Sentiment Analysis Lexicons?

Sentiment analysis lexicons are collections of words or phrases, each associated with a sentiment score or label. These lexicons help in assigning sentiment values to words in a text, which can be aggregated to determine the overall sentiment of the text. They are commonly used in various sentiment analysis applications, including social media monitoring, customer feedback analysis, and opinion mining.

## Examples of Lexicons

Here are some notable sentiment analysis lexicons:

### 1. [MPQA Subjectivity Lexicon](https://mpqa.cs.pitt.edu/#subj_lexicon)

- **Description:** The MPQA (Multi-Perspective Question Answering) Subjectivity Lexicon contains words and phrases annotated with subjectivity scores. It provides insights into the subjectivity or objectivity of text and is useful for sentiment analysis and opinion mining.
- **Resource:** [MPQA Subjectivity Lexicon](https://mpqa.cs.pitt.edu/#subj_lexicon)

### 2. [Bing Liu and Minqing Hu Sentiment Lexicon](https://www.cs.uic.edu/%7Eliub/FBS/sentiment-analysis.html#lexicon)

- **Description:** This lexicon, developed by Bing Liu and Minqing Hu, is one of the earliest sentiment lexicons. It includes a list of positive and negative words, making it a valuable resource for basic sentiment analysis tasks.
- **Resource:** [Bing Liu and Minqing Hu Sentiment Lexicon](https://www.cs.uic.edu/%7Eliub/FBS/sentiment-analysis.html#lexicon)

### 3. [SentiWordNet](https://github.com/aesuli/SentiWordNet) (Included in NLTK)

- **Description:** SentiWordNet is a lexical resource for sentiment analysis that assigns sentiment scores to WordNet synsets. It provides positive, negative, and objective scores for each synset, allowing for fine-grained sentiment analysis.
- **Resource:** [SentiWordNet](https://github.com/aesuli/SentiWordNet) (Included in NLTK)

### 4. [VADER Sentiment Lexicon](https://github.com/cjhutto/vaderSentiment/blob/master/vaderSentiment/vader_lexicon.txt)

- **Description:** VADER (Valence Aware Dictionary and sEntiment Reasoner) is a sentiment lexicon designed for social media text. It includes a set of words with associated sentiment scores and is particularly effective for analyzing sentiment in short texts, such as tweets and reviews.
- **Resource:** [VADER Sentiment Lexicon](https://github.com/cjhutto/vaderSentiment/blob/master/vaderSentiment/vader_lexicon.txt)

### 5. [SenticNet](https://sentic.net/)

- **Description:** SenticNet is a sentiment lexicon that incorporates both sentiment and conceptual information. It provides sentiment scores along with semantic concepts, allowing for more nuanced sentiment analysis and understanding of text.
- **Resource:** [SenticNet](https://sentic.net/)

## How to Use Sentiment Analysis Lexicons

1. **Select a Lexicon:** Choose a lexicon that suits your analysis needs based on factors such as language, domain, and granularity of sentiment information.
2. **Preprocess Text:** Clean and preprocess your text data by removing noise and normalizing text.
3. **Tokenize Text:** Split the text into tokens (e.g., words or phrases) to match with entries in the lexicon.
4. **Assign Sentiment Scores:** Use the lexicon to assign sentiment scores to each token.
5. **Aggregate Scores:** Combine the sentiment scores to determine the overall sentiment of the text.

## Conclusion

Sentiment analysis lexicons are powerful tools for understanding and analyzing emotions in text. By leveraging these lexicons, you can gain insights into public opinion, customer feedback, and various other applications. The examples provided offer a starting point for exploring sentiment analysis lexicons and integrating them into your NLP workflows.

For a detailed tutorial on how sentiment analysis lexicons work, you can refer to the [Sentiment Symposium Tutorial by Christopher Potts](http://sentiment.christopherpotts.net/lexicons.html).



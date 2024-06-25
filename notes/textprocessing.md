---
layout: page
title: Tasks for text processing
nav_exclude: true
permalink: /notes/textprocessing/
---

# Tasks for text processing

Removing stopwords <br>
Performing normalization tasks  <br>
Stemming  <br>
Performing lemmatization  <br>
Tagging parts of speech  <br>
Performing tokenization  <br>


## Remove stopwords
***Example of a raw text:*** Text preprocessing is an important NLP step b4 training a model. Tasks to correct speling, converting words to a better standard form & removing STOPWORDS.

***Remove stopwords:*** <br>
Task 3: Text preprocessing <span style='background-color: yellow;'>~~is an~~</span> important NLP step b4 training <span style='background-color: yellow;'>~~a~~</span> model. Tasks <span style='background-color: yellow;'>~~to~~</span> correct speling, converting words <span style='background-color: yellow;'>~~to a~~</span> better standard form & removing STOPWORDS. <br>
Stopwords removed in the example: “Is an”, "a", “to”, “to a”

## Normalization
Performing text normalization includes removing punctuations, converting numbers to text, and, converting text to lowercase.

***Example after stopwords removal*** <br>
Task 3: Text preprocessing important NLP step b4 training model. Tasks correct speling, converting words better standard form & removing STOPWORDS. <br>

***Normalize***<br>
<span style='background-color: yellow;'>t</span>ask <span style='background-color: yellow;'>three</span> <span style='background-color: yellow;'>t</span>ext preprocessing important <span style='background-color: yellow;'>natural language processing</span> step <span style='background-color: yellow;'>before</span> training model <span style='background-color: yellow;'>t</span>asks correct <span style='background-color: yellow;'>spelling</span> converting words better standard form removing <span style='background-color: yellow;'>stopwords</span>
<br>
After normalization, punctuations are removed, all text is now lowercase. NLP acronym is spelled out. “b4” becomes “before”. Punctuation is removed and “speling” is corrected as “spelling”.













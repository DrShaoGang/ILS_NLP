---
layout: page
title: What's Natural Language Processing (NLP)?
nav_exclude: true
permalink: /notes/whatsnlp/
---

# What's Natural Language Processing (NLP)?


## Natural Language Processing 
Natural language processing is a field of science and engineering focused on the development and study of automatic systems that understand and generate natural (that is, human,) languages. 

## Humans and language 
Human languages are communicative devices enabling the efficient sharing and storage of complex ideas, facts, and intents. As [Manning, 2022](https://www.amacad.org/publication/daedalus/human-language-understanding-reasoning) argues, the complexity of communication enabled by language is a uniquely human intelligence among species. As scientists and engineers interested in the creation and study of intelligent systems, human language is to us both a fascinating object of study—after all, it has evolved to be learnable and useful—and a great enabler for interacting with humans even in contexts where other modalities (e.g., vision) are also of interest. 

## Language and machines 
Human children, interacting with a rich multi-modality world and various forms of feedback, acquire language with exceptional sample efficiency (not observing that much language) and compute efficiency (brains are efficient computing machines!) With all the (impressive!) advances in NLP in the last decades, we are still nowhere close to developing learning machines that have a fraction of acquisition ability of children. One fundamental (and still quite open) problem in building language-learning machines is the question of representation; how should we represent language in a computer such that the computer can robustly process and/or generate it? This is where this course focuses on the tools provided by deep learning, a highly effective toolkit for representing both the wild variety of natural language and some of the rules and structures it sometimes adheres to. Much of this course will be dedicated to this question of representation, and the rest of this note will talk about a basic subquestion: how do we represent words? Before that, though, let’s briefly discuss some of the applications you can hope to build after learning modern NLP techniques.

## NLP example
<div class="fig figcenter fighighlight">
  <img src="/ILS_NLP/assets/images/alexa.jpg" width="40%" alt="ask questions to alexa"> 
  <div class="figcaption"> NLP example: “Alexa, what’s it like outside?”
</div>
</div>
Here is a diagram of how Amazon Alexa uses NLP to create a conversation with users. First, an Amazon device, such as an Echo, records your words. The recording of your speech is sent to Amazon servers to be analyzed more efficiently. Amazon breaks down your phrase into individual sounds. Then, it connects to a database that contains the pronunciations of various words to find which words most closely correspond to the combination of individual sounds. Then, Alexa identifies important words to make sense of the tasks and to carry out corresponding functions. For instance, if Alexa notices words like outside or temperature, it opens the weather app. Finally, Amazon servers send the information back to your device, and Alexa speaks.



## NLP workflow

<div class="fig figcenter fighighlight">
  <img src="/ILS_NLP/assets/images/NLP_language_structure.jpg" width="60%" alt="NLP language structure"> 
</div>

NLP develops computational algorithms to analyze and represent human language automatically. Many NLP systems now use some form of machine learning. NLP works with the hierarchical structure of language. Words are at the lowest layer of the hierarchy. A group of words makes a phrase. The next level up in the hierarchy is a group of phrases, which make a sentence, and ultimately, sentences convey ideas. 








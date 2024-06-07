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
Human languages are communicative devices enabling the efficient sharing and storage of complex ideas, facts, and intents. As [Manning, 2022] argues, the complexity of communication enabled by language is a uniquely human intelligence among species. As scientists and engineers interested in the creation and study of intelligent systems, human language is to us both a fascinating object of study—after all, it has evolved to be learnable and useful—and a great enabler for interacting with humans even in contexts where other modalities (e.g., vision) are also of interest. 

## Language and machines 
Human children, interacting with a rich multi-modality world and various forms of feedback, acquire language with exceptional sample efficiency (not observing that much language) and compute efficiency (brains are efficient computing machines!) With all the (impressive!) advances in NLP in the last decades, we are still nowhere close to developing learning machines that have a fraction of acquisition ability of children. One fundamental (and still quite open) problem in building language-learning machines is the question of representation; how should we represent language in a computer such that the computer can robustly process and/or generate it? This is where this course focuses on the tools provided by deep learning, a highly effective toolkit for representing both the wild variety of natural language and some of the rules and structures it sometimes adheres to. Much of this course will be dedicated to this question of representation, and the rest of this note will talk about a basic subquestion: how do we represent words? Before that, though, let’s briefly discuss some of the applications you can hope to build after learning modern NLP techniques.

<div class="fig figcenter fighighlight">
  <img src="/assets/images/alexa.jpeg" width="40%">
  <div class="figcaption"> NLP example: “Alexa, what’s it like outside?”
</div>
</div>

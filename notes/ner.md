---
layout: page
title: Name Entity Recognition (NER)
nav_exclude: true
permalink: /notes/ner/
---


# Name Entity Recognition (NER)

Name Entity Recognition (NER) is a subtask of natural language processing (NLP) that aims to identify and classify named entities (proper nouns) into predefined categories such as person names, organization names, locations, dates, numerical values, and more. NER is crucial for extracting meaningful information from unstructured text and is used in various NLP applications such as information retrieval, question answering, and sentiment analysis.

## How NER Works

NER typically involves the following steps:

1. **Tokenization**: Breaking down text into individual tokens (words or phrases).
   
2. **Part-of-Speech (POS) Tagging**: Assigning a grammatical category (like noun, verb, adjective) to each token.

3. **Named Entity Recognition**: Identifying tokens that are names or entities and classifying them into predefined categories.

## Types of Named Entities

Common types of named entities that NER systems can identify include:

- **Person**: Individuals' names.
- **Organization**: Names of companies, institutions, etc.
- **Location**: Names of places, cities, countries, etc.
- **Date**: Specific dates or periods of time.
- **Number**: Numerical quantities.
- **Miscellaneous**: Other types like product names, events, etc.

## Example

Consider the following sentence:

*"Apple Inc. is headquartered in Cupertino, California, and was founded by Steve Jobs."*

NER would identify the following named entities:

- **Organization**: Apple Inc.
- **Location**: Cupertino, California
- **Person**: Steve Jobs

## NER in Python Example

Here's a simple Python example using the popular library spaCy for NER:

```python
import spacy

# Load the English NER model
nlp = spacy.load("en_core_web_sm")

# Example text
text = "Apple Inc. is headquartered in Cupertino, California, and was founded by Steve Jobs."

# Process the text with spaCy
doc = nlp(text)

# Print identified entities
for ent in doc.ents:
    print(f"Entity: {ent.text}, Type: {ent.label_}")

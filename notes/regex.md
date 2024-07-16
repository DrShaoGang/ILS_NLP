---
layout: page
title: Regular Expression
nav_exclude: true
permalink: /notes/regex/
---

# Regular Expression for Information Extraction
# Regular Expressions (Regex) 

Regular expressions (regex) are powerful tools for pattern matching and text manipulation. In NLP, regex is commonly used to identify and extract specific patterns of text, such as dates, email addresses, URLs, and more. They provide a flexible and efficient way to process textual data based on predefined rules.

## Basics of Regular Expressions

Regular expressions consist of sequences of characters that define a search pattern. Here are some basic elements used in regex:

- **Literal characters**: Characters that match themselves (e.g., `a`, `1`, `@`).
- **Metacharacters**: Characters with special meanings in regex, such as `.`, `*`, `+`, `?`, `[`, `]`, `{`, `}`, `^`, `$`, `|`, `\`.

## Common Use Cases in NLP

### 1. Pattern Matching

Regex allows us to search for specific patterns within text data. For example, identifying email addresses or detecting mentions of dates in textual documents.

```python
import re

# Example text
text = "Contact us at email@example.com or support@domain.com for assistance."

# Regex pattern to match email addresses
pattern = r'\b[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\.[A-Z|a-z]{2,}\b'

# Find all email addresses in the text
emails = re.findall(pattern, text)

print("Email addresses found:", emails)


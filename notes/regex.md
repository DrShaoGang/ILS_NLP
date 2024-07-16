---
layout: page
title: Regular Expression
nav_exclude: true
permalink: /notes/regex/
---

# Regular Expression for Information Extraction

Regular expressions (regex) are powerful tools used for pattern matching and text processing. In the context of Natural Language Processing (NLP), regex can be particularly useful for tasks such as:

- **Tokenization**: Breaking text into individual tokens (words or phrases).
- **Text Cleaning**: Removing unwanted characters, punctuation, or formatting.
- **Pattern Matching**: Identifying specific patterns or structures within text data.
- **Entity Recognition**: Extracting entities like dates, email addresses, or phone numbers.

## Basic Syntax

Regex consists of special characters and sequences that define patterns. Here are some fundamental elements:

- `.` - Matches any single character except newline.
- `\d` - Matches any digit (0-9).
- `\w` - Matches any alphanumeric character (equivalent to `[a-zA-Z0-9_]`).
- `[ ]` - Matches any single character within the brackets.
- `|` - Alternation, matches either the expression before or after the pipe.
- `^` - Matches the start of a line.
- `$` - Matches the end of a line.



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
```
## Text Cleaning and Tokenization
Regex helps in cleaning and preprocessing text by removing unwanted characters, normalizing text (e.g., converting to lowercase), and tokenizing text into words or sentences.
```python
#Example: Removing Punctuation
import re

text = "Hello, World! How are you?"
clean_text = re.sub(r'[^\w\s]', '', text)
print(clean_text)
# Output: Hello World How are you
```
### Explanation:
- "[^\w\s]": Matches any character that is not a word character (\w) or whitespace (\s), effectively removing punctuation from the text.


---
layout: page
title: Types of text extraction
nav_exclude: true
permalink: /notes/textextraction/
---

# Types of text extraction

## Unstructured Data

### Raw Text
- Extracting plain text from documents or web pages without any specific formatting.

Example:
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.

### Words or Sentences Extraction
- Identifying and extracting specific words or sentences from unstructured text.

Example:
Extracted sentence: "consectetur adipiscing elit."

## Image Data

### Extract Text from Images
- Using OCR (Optical Character Recognition) to extract text from images.

Example:
<div class="fig figcenter fighighlight">
  <img src="/ILS_NLP/assets/images/purduegate.jpg" width="40%" alt="an image of Purdue gate"> 
</div>
Extracted text: "Purdue University."

## Structured Data

### Tabular Data
- Extracting structured data from tables, such as banking records or employment records.

Example:

| Date       | Description        | Amount |
|------------|--------------------|--------|
| 2023-01-01 | Salary Deposit     | $5000  |
| 2023-01-05 | Rent Payment       | $1200  |
| 2023-01-10 | Utilities Payment  | $200   |



### Forms Data
- Reading and extracting structured data from forms.

Example:
Form Data:
- Name: John Doe
- Age: 30
- Address: 123 Main Street
- City: Anytown
- State: NY

Extracted Data:
{
  "Name": "John Doe",
  "Age": 30,
  "Address": "123 Main Street, Anytown, NY"
}


## Conclusion
Effective text extraction techniques are essential for transforming raw data into actionable insights. By understanding the different types of data and the corresponding extraction methods, you can leverage text extraction to improve data analysis and decision-making processes.

# Nepali CFG Parser

A simple, rule-based Context-Free Grammar (CFG) parser for the Nepali language, built using Python and NLTK.

## Overview
This project was developed to map and parse the grammatical structure of basic Nepali sentences. Unlike English, which follows a Subject-Verb-Object (SVO) structure, Nepali typically follows a **Subject-Object-Verb (SOV)** structure. This parser uses a custom lexicon and grammar rules to generate syntax trees for valid Nepali sentences.

## Features
* **Rule-Based Parsing:** Utilizes NLTK's `ChartParser` to evaluate sentences against predefined CFG rules.
* **SOV Architecture:** Specifically designed to recognize Subject-Object-Verb phrasing (e.g., Noun Phrase + Noun Phrase + Verb).
* **Automated Evaluation:** Includes a test script to evaluate model accuracy against a dataset of valid and invalid sentence structures.

## Dependencies
* Python 3.x
* NLTK (`pip install nltk`)

## Usage
1. Clone the repository.
2. Run the Python script or open the Jupyter Notebook / Google Colab file.
3. The parser will output a visual representation of the parse tree.

```python
import nltk

# Example usage
sentence = "रामले स्याउ खायो".split()
for tree in parser.parse(sentence):
    tree.pretty_print()


# 20th Century Network Analysis – Exercise 1.4

This project involves web scraping data from the Wikipedia page **Key Events of the 20th Century** as part of the CareerFoundry Data Analytics program.

## Overview
The goal was to collect text data about major world events in the 20th century.  
This scraped text will later be used for text mining and network analysis.

## Data Source
- [Wikipedia: Key events of the 20th century](https://en.wikipedia.org/wiki/Key_events_of_the_20th_century)

## Tools
- Python  
- Requests  
- BeautifulSoup  
- JupyterLab  

## Files
- `20th_century_scrape.ipynb` – notebook used to scrape and save data  
- `20th_century_events.txt` – text output file  
- `README.md` – project summary  

---
# Exercise 1.5 – Text Mining Analysis
# Overview
This exercise analyzes text scraped from the Wikipedia page “Key Events of the 20th Century.”
The goal was to clean the text, tokenize it, analyze frequencies, run POS tagging, and check how often countries were mentioned.
# Steps Completed
1.Load the Scraped Text
Loaded the text file from Exercise 1.4
Previewed the first part to confirm successful loading
2. Tokenization & Word Frequency
Tokenized the full text
Removed punctuation and stopwords
Created bar plots of the Top 10 Most Common Words (before and after cleaning)
3.  POS Tagging with TextBlob
Generated POS tags for each word
Identified the Top 10 POS tags
# Plotted:
Top 15 nouns
Top 15 verbs
Top 15 adjectives
4. Country Mention Frequency
Used a list of 190+ countries
Counted how often each country appeared
Created a dataframe of country frequencies
Plotted the distribution of mentions
# Key Findings
After removing stopwords, meaningful words like war, world, and history appear most frequently
Nouns dominate the POS distribution — expected for a historical article
Some countries appear much more (e.g., Vietnam, Australia, Ukraine) due to major 20th-century events
Most countries were mentioned only once
# Files Included
text_mining.ipynb — analysis notebook
20th_century_events.txt — scraped text
README.md — project documentation


# Exercise 1.6 – NLP & NER Analysis

For this exercise, I used Natural Language Processing to analyze the twentieth-century events text from Exercise 1.4. I created an NER object using spaCy, split the text into sentences, and filtered the entities to keep only country-related items (GPE/LOC). I then identified sentences where two or more countries appeared together and used this information to build a relationships dataframe. These outputs will be used to create the network visualization in Exercise 1.6.

### Files Created
- `exercise_1_6_nlp.ipynb`
- `20th_century_events_clean.txt`
- `country_relationships.csv`

# large dictionary for geographical classification of news in Russian
# current version: 11 527 entries

·for each country, the names of the major cities and regions were scraped from RussianWikipedia;
·all the words were stemmed using the Porter Stemmer;
·entries with the initial length of greater or equal to 6 symbols were concatenated with “*”;
·entries with the initial length of less than 6 symbols were concatenated with “*” or “?”manually depending on the word’s part of speech;
·stemmed tokens matching stopwords were removed;·if a duplicate entry occurred in a dictionary, a geographical name for an item with smallerpopulation was dropped.
Note:
The dictionary is designed in a way that pattern matching "glob" will create less ambiguity than "regex"



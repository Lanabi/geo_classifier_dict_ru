# large dictionary for geographical classification of news in Russian
# current version: 11 527 entries

How it was created:

1) for each country, the names of the major cities and regions were downloaded from Wikipedia
2) all the words were stemmed with Porter Stemmer
2) words with initial length  >= 6 symbols:  stems were concatenated with '*' symbol
3) words with initial length  < 6 symbols: stems were checked and concatenated with '*' or '?' manually
4) if the stem of a word matched the stem of one of 5000 most commonly words in Russian, the stem was dropped from the dictionary
5) if a duplicate entry occurred in a dictionary, a geographical item which population is less was dropped

Note:
The dictionary is designed in a way that pattern matching "glob" will create less ambiguity than "regex"



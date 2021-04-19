# large dictionary for geographical classification of news in Russian
# current version: 11 527 entries

How was it created?

1) for each country, the names of the major cities and regions were downloaded from Wikipedia
2) all the words were stemmed with Porter Stemmer
2) words with initial length  >= 6 symbols:  stems have been concatenated with '*' symbol
3) words with initial length  < 6 symbols: stems have been checked manually and concatenated with '*' or '?' 
4) if the stem of a word matched the stem of one of 5000 most commonly words in Russian, the has baan dropped from the dictionary

Note:
The dictionary is designed in a way that pattern matching "glob" will create less ambiguity than "regex"



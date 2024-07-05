# Web-Corpus-Generator using the Web
This work is supported by the Ministry of Higher Education and Scientific Research in Algeria (Project C00L07UN100120180002) 

Conception & Supervision: L. Ouahrani & D. Bennouar / Contributor: Abdennour BenHamida.

This code allows to generation of a corpus from the web based on keywords related to the subject of the study, cleaned and ready to use. The corpus will be stored in a JSON file in the same path as the "WebCorp.py" is running. The output contains:

- Corpus Name
- Words count: total number of words and different words
- Articles count: number of web articles returned into the corpus
- Articles: a dictionary containing all the textual data returned stored as { Article's title: Content}

1- Requirments: 
- You may need to enable these two commands if your punkt isn't installed, once downloaded and installed nltk will work perfectly fine:
  #1- import nltk
  #2- nltk.download('punkt')
- Python 2.7 or later
- Internet connection
- At least 20mb of free storage

2- Libraries used:
- Bs4: BeatifulSoup4 is a Python library used for web scrapping (extracting web content from HTML or XML pages)
- re.sub: a function that allows as to delete portions of text that are or not in the text
- word_tokenize: we use to tokenize (split) our texts into a list of words
- request exception to handle connection errors and timeouts
- sleep for time out exception handling
- langdetect: a tool that detects languages, so that we don't return any article that is not written in Arabic
- json: storing results

3- How to use:
- Call the "toJson" function with its two parameters:
  - Keywords: a string with words describing your research or a subject (a bigger keychain leads to a much more detailed corpus and richer content)
  - Name: name of the JSON file that will be created after generation
- The more keywords you insert, the bigger and more precise the corpus will be
 
 For further questions or inquiries about this code, you can contact l_ouahrani@univ-blida.dz
 
 

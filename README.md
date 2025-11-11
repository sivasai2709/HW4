# HW4
#Q1 This project demonstrates a basic Natural Language Processing (NLP) pipeline in Python using the
spaCy library. The goal of the program is to take an input sentence and process it through several
text-cleaning steps to extract meaningful words. The steps included are tokenization, stopword
removal, lemmatization, and part-of-speech filtering. Tokenization breaks the sentence into
individual words or tokens. Stopword removal eliminates common words such as “the”, “is”, and “in”
that do not contribute significant meaning. Lemmatization converts words to their root form, such as
changing “playing” to “play”. Finally, only nouns and verbs are retained by checking the POS
(Part-of-Speech) tags assigned by spaCy.
The example input sentence used is: “John enjoys playing football while Mary loves reading books
in the library.”
After processing, the output is a list of meaningful lemmas that represent the key concepts in the
sentence: ['john', 'enjoy', 'play', 'football', 'mary', 'love', 'read', 'book', 'library']
This shows that names, actions, and objects are preserved while unnecessary connecting words
are removed.

#Q2
# Pronoun Ambiguity Detection Using spaCy

This project demonstrates how to detect named entities and identify pronoun ambiguity in a sentence using the spaCy natural language processing library. The script processes a given sentence to recognize names of people, organizations, places, and products through Named Entity Recognition (NER). After identifying entities, the program checks the text for the presence of third-person pronouns such as “he”, “she”, “they”, “him”, “her”, or “them.” These pronouns can sometimes make sentences unclear because it may not be obvious who the pronoun is referring to. When such pronouns are detected, the program displays a warning message, indicating that the sentence may contain ambiguous references.

The example sentence used is:  
“Chris met Alex at Apple headquarters in California. He told him about the new iPhone launch.”  
In this case, both “He” and “him” could refer to either Chris or Alex, making the meaning unclear. The script correctly detects this and warns about possible pronoun ambiguity. This type of analysis is useful in applications such as text editing tools, chatbots, summarization systems, and early-stage coreference resolution research.



# Poetry Generation in Urdu
In this work, I used n-gram language modeling to generate some poetry using the spaCy library for
text processing. Each poem consists of four stanzas each containing three
verses where each verse consists of 7—10 words. 

The task is to print four such stanzas with an empty line in between. The generational model can be trained
on the provided Poetry Corpus containing poems from Faiz, Ghalib and Iqbal. I've trained unigram and
bigram models using this corpus. These models will be used to generate poetry.

Assignment Task
The task was to generate a poem using different models. We will generate a poem verse by verse until all stanzas
have been generated. The poetry generation problem is solved using the following algorithm:


1. Load the Poetry Corpus
2. Tokenize the corpus in order to split it into a list of words
3. Generate n-gram models
4. For each of the stanzas
  – For each verse
    * Generate a random number in the range [7...10]
    * Select first word
    * Select subsequent words until end of verse
    * Print verse
  – Print empty line after stanza

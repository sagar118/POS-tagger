# POS-tagger

A Part-Of-Speech Tagger (POS Tagger) is a piece of software that reads text in some language and assigns parts of speech to each word (and other token), such as noun, verb, adjective, etc. Develop a POS tagger using HMM and Viterbi Algorithm. Also, modify the vanilla Viterbi Algorithm to handle the unknown words.

Viterbi Algorithm fails to tag words that were not present in the training corpus since the emission probabilities for those words are zero.

To overcome this problem we modified the Viterbi Algorithm using three methonds:

1. RegexpTagger
2. Lexicon based
3. Laplace Smoothing

Out of the three Regex based showed the most improvement as we can identify words using the common suffixes for different tags but it still fails to tag words based on the context. After regex based viterbi algorithm lexicon performance was better than vanilla viterbi algorithm. In the end laplace smoothing showed some improvement but it was small.

# Hadoop

This repository includes few algorithms that are implemented in Hadoop environment on the Gutenberg dataset.

The following map-reduce algorithms are implemented on the Hadoop framework.

#1 Produce count of every single word in the gutenberg document.
Files - count_mapper.py | count_reducer.py

#2 Implement MapReduce algorithm to produce inverted index for the whole dataset.
Files - inverted_mapper.py | inverted_reducer.py

#3 Implement MapReduce algorithm to produce modified trigrams around a certain keywords after replacing the keyword with '$'.
   Example : cat was sitting on a roof ---> if the key word was ‘sitting’ ---> the modified tri-grams would be cat_was_$, was_$_on,$_on_a,.
   The key words to look for in the gutenberg dataset are ‘science’, ‘sea’ , ‘fire’. 
   The algorithm after producing these modified tri-grams,  should return the 10 most occurred modified tri-gram in the dataset.
Files - trigram_mapper.py | trigram_reducer.py | trigram_mapper2.py | trigram_reducer2.py

# spell_checker_trie
A spell checker using trie data structure in C, Time and space complexity tested

Trie functioning:

1. Loading:
	a. We parsed a text file with all the dictionary words.
	b. In the dictionary file, each word is followed by a newline character. 
	c. When we encounter a newline character, we do boolean true for 	the trie path, else we 	    keep traversing the trie.
	d. Each letter of a word corresponds to an index in the array of pointers in a trie node.

2. Checking:
	a. We parse the file, each word is distinctly recognized by the placement of 		    punctuations and newlines. Special characters are ignored.
	b. Whenever anything apart from an alphabet is encountered, we pass the word into the 	    checker function and check the return type.
	c. In the checker function, we retrace the trie according to the string argument.
	d. After the string has ended, we check if the child node returns boolean true or false. If 	    its true, the word is correct else its incorrect.
	
3. Unload:
	a. Here we go through a recursive process of deallocating memory 	for all the nodes that 	    are leaf nodes of the corresponding sub-tries

CONCLUSION:
Implementing a spell checker using a trie is more efficient than most data structures in most languages. The code seems tedious but the speed and accuracy compensate for it. So, we can detect spelling errors in documents without cumbersome reading.



- talk about how to access FORTH and how to exit it
- talks about the basic input buffer, the back space , and the delete key
- take an example of 1 . 1 ok to show how the input buffer works , how it first takes it as a word in the dictionary and search it, as 1 is a primtive keywork, it will push the 1 into the stack, then it will search for the next word, which is ., and it will search for the word in the dictionary, and it will find it, and it will execute the word, which will pop the top of the stack, and print it, and then it will print ok

- any error of a word that is not in the dictionary will be printed as an error messae will result in the partially compiled keyword being removed from the dictionary.

#### Dictionary Format



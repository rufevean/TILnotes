## Threaded Interpretive Languages

### Introduction

- the goal is to reverse the trend of increasing complexity in programming Languages
- A threaded interpreter approach is used to implement a simple language that is easy to understand , extend and modify.
- TILs can be used to implement a micro computer monitor, a general purpose programming language , an editor etc etc

#### What is a TIL?

- There are many types of translators that convert a high level language into machine code. if the source language is a high level language and the target language is machine code, the translator is called a compiler. If the source code is directly executed without converting into a machine language,its called an interpreter.

###### Explaining a threaded coded interpreter ( by my mentor)

>there will be a bed (as in strawberry bed) of CFAs (code field address) sequentially imbedded in a row in what Forth calls the “dictionary”, but i will refer to as the “lex” (short for “lexicon”).
Each CFA is an executable function pointer of what Forth calls “a colon word” (which means a “word” that was defined in Forth).
So each CFA represents the executable address of a “word” (what i will call a “lexal”).
So to summarize, a lexal is a word defined in the TIL language, each lexal definition is stored in the lex.  Each lexal itself has a PFA (parameter Field Address) which is a bed of CFAs to previously defined lexals.
The threaded code interpreter sequentially executes each CFA in the PFA of a lexal.

thanks for the explanation. 


- it uses reverse polish notation(RPN) to represent the instructions. they are highly efficient and easy to implement. The use of the data stack and RPM allows as easy left to right scan of an input line. As each number is scanned , its value is pushed onto the stack and when there is an operator, the operator is executed using the operands on the stack.




#### Elements of a TIL 

- The TIL consists of a number of elements. Lets start with tokens . Tokens are the smallest unit of a language. They are the building blocks of a language. Tokens are used to represent the keywords, identifiers, constants, operators etc. 

> carriage return : means the end of a line and the beginning of a new line.

- An input line consists of a sequence of tokens separated by white spaces and ended by a carriage return.

- successful comletion of an input operation is usually followed by the system ecohing a message to the user. "ok" is the usual message.

- every input is stored in UPPER CASE.

The main Elements of a TIL is its Dictionary. The dictionary is a list of words and their corresponding addresses. The dictionary is used to look up the address of a word when it is encountered in the input line 

- Dictionary contains two types of words : 

     - core words : these are the basic words that are used to implement the language. They are the building blocks of the language.

     - user defined words : these are the words that are defined by the user. They are used to extend the language.


- Tils use stacks, specfically two stacks. The data stack and the return stack. The data stack is used to store the data like numbers and addresses of the operands. the return stack is used to store program flow control parameters .  




#### The attributes of a TIL 

- A threaded imterpretive language is gernerally fast compared to most ineterprets available for microcomputers.
but they are slow relative to optimal assembled code.

- A major advantage of a TIL is the memory required to implement the language . the core language can be contained in less than 4k bytes of memory and an assembler, editor and virtual memory system requires an additional 2-3 k byes .


- one of the nicest features of a TIL is the simplicity with which programs can be developed and tested.

- the only difficulty feature is tracking the order and number of items on the stack. 

#### Implementation Notes

- There are two types of keyword structures in a TIL. Primitives and secondaries.

- primitives are closely akin to subroutines. secondaries are akin to a list of subroutines. 

- There are several ways to handle different data types. the philosophy adopted for the TIL will be substantially different. All operators will presume operands of a give type. for example, the operator + will presume that the operands are integers. the opearator F+ will presume that the operands are floating point numbers.




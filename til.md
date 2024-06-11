## Threaded Interpretive Languages

### Introduction

- the goal is to reverse the trend of increasing complexity in programming Languages
- A threaded interpreter approach is used to implement a simple language that is easy to understand , extend and modify.
- TILs can be used to implement a micro computer monitor, a general purpose programming language , an editor etc etc

#### What is a TIL?

- There are many types of translators that convert a high level language into machine code. if the source language is a high level language and the target language is machine code, the translator is called a compiler. If the source code is directly executed without converting into a machine language,its called an interpreter.


- a threaded code interpreter is a type of interpreter that uses a stack to store the address of the next instruction to be executed. The interpreter fetches the next instruction from the stack and executes it. The interpreter continues to fetch and execute instructions until the stack is empty. 
-
it uses reverse polish notation(RPN) to represent the instructions. they are highly efficient and easy to implement.




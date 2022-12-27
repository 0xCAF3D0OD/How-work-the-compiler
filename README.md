# How-work-the-compiler

## Introduction
Do you know how the compiler works, no?! Neither do I, so I made this article to understand how it really works.

## CPU
* the processor(`CPU` or Central Processing Unit) is the logic circuity that respond to basic instructions that make the computer running. **The brain of the computer**

* at a low level, computer processor can only do a small number of things.
  1. they can read and write to memory.
  2. they can do math with number they are holding.

## Executable Program
* Is generated by the compiler is a list of instructions for the processor to follow, the are written in binary. this instruction are called **machine code**

* A hex dump of an executable real mode loader   
* <img src="https://upload.wikimedia.org/wikipedia/commons/2/29/Binary_executable_file2.png" width="150">

* When we talk about programming we talk about high level programming with condition, loop, etc..., all that is for make the work easier for the humans to understand it and this is called **source code**.
* that is called source code.
* <img src="https://www.tldevtech.com/wp-content/uploads/2021/07/source-code.jpg" width="150">
* the compiler take this **source code** and transforme it in **machine code**.

### Sources to machine code
* What happens when you go from source code to compiler? For the compiler, the source code is only meiningless text.
* First the compiler search for preprocessing directive. 
1. **He divides** the code in individual **tokens**.
2. **He figuring out** what for **words are in the program**.
3. Tokens are organized into a hierachical structure (parse tree), figuring what "grammar" is in program.
4. The compiler register contexe about program (including variable and function names).
5. He traverse the tree and figure out if some machine code would make the same thing as the source code
* After all this stuff the compiler has finaly his machine code for understand your code.
    - Ex if you want to assigne to an integer the value 3, the compiler will stock the value in the memory with his particular machine code.
* If you change the source code the compiler will do de same route but with the change init a stock the new value in the memory.

## How it's works with the conditions
in working...
## references

[processor (CPU)] (https://www.techtarget.com/whatis/definition/processor)

# How-work-the-compiler

### Introduction
* >Do you know how the compiler works, no?! Neither do I, so I made this article to understand how it really works.

### CPU
* The processor (`CPU` or Central Processing Unit) is the **logic circuity** that respond to basic instructions that make 
the computer running. **The brain of the computer**

* at a low level, computer processor can only do a small number of things.

  * They can read and write to memory.
  * They can do math with number they are holding.


   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
   [<img src="img/processor.jpg" width="250">](img/processor.jpg)

[//]: # (   [![processor appearance]&#40;<img src="img/processor.jpg" width="250">&#41;]&#40;img/processor.jpg&#41;)


### Executable Program
* Is generated by the compiler is a list of instructions for the processor to follow, they are written in binary. 
This instruction are called **machine code**

* A hex dump of an executable real mode loader   
   

   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
   [<img src="https://upload.wikimedia.org/wikipedia/commons/2/29/Binary_executable_file2.png" width="250">](<img src="https://upload.wikimedia.org/wikipedia/commons/2/29/Binary_executable_file2.png" width="1500">)

[//]: # ([![hex dump example]&#40;<img src="https://upload.wikimedia.org/wikipedia/commons/2/29/Binary_executable_file2.png" width="250">&#41;]&#40;<img src="https://upload.wikimedia.org/wikipedia/commons/2/29/Binary_executable_file2.png" width="1500">&#41;)

* When we talk about programming we talk about high level programming with condition, loop, etc..., 
all that is for make the work easier for the humans to understand it and this is called **source code**.
* that is called **source code**.


   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
   [<img src="img/codebrowser_kdevelop.png" width="250">](img/codebrowser_kdevelop.png)

[//]: # (   [![source code example]&#40;<img src="img/codebrowser_kdevelop.png" width="250">&#41;]&#40;img/codebrowser_kdevelop.png&#41;)


* the compiler take this **source code** and transforme it in **machine code**.

### Sources to machine code
* >What happens when you go from source code to compiler? For the compiler, the source code is only meaningless text.
1. **Preprocessing step:** The compiler search for preprocessing directive `(#include)`.
   * The directive are **preceded by the "#" sign**.
   * If a directive is found, she is directly treated and the compiler insert the content of the file in the directive.
   * All the directive have been treated, the compiler has a modified version of source code, ready for compilation.


   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
   [<img src="img/Diagram_preprocessor.png" width="250">](img/Diagram_preprocessor.png)

[//]: # (   [![pre-processor scheme]&#40;<img src="img/Diagram preprocessor.png" width="250">&#41;]&#40;img/Diagram_preprocessor.png&#41;)


2. **Lexical analysis:** He divides the code in individual **tokens**.
   * Each token has a **lexical unit** (keyword or symbol for example).
   * The token **syntax is a rational language** who is recognisable by the compiler.


   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
   [<img src="img/analyzer.png" width="350">](img/analyzer.png)

[//]: # (   [![lexical analyser scheme]&#40;<img src="img/analyzer.png" width="300">&#41;]&#40;img/analyzer.png&#41;)


3. **He's figuring out** what for **words are in the program**.
4. Tokens are organized into a hierarchical structure (parse tree), figuring what "grammar" is in program.
5. The compiler register context about program (including variable and function names).
6. He traverse the tree and figure out if some machine code would make the same thing as the source code
* After all this stuff the compiler has finally his machine code for understand your code.
    - Ex if you want to assign to an integer the value 3, the compiler will stock the value in the memory with his particular machine code.
* If you change the source code the compiler will do de same route but with the change init a stock the new value in the memory.

## How it's works with the conditions
in working...
## references

[processor (CPU)] (https://www.techtarget.com/whatis/definition/processor)

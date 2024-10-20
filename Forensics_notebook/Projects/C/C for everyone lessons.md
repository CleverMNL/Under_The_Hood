These are adapted notes from a course on C. Developed by Dennis Richie in 1972 (72!). 

---
Module 1 video 1 Compiler run through

To write code, you need a text editor. An editor includes things like Notepad, Word (this is an "intelligent" or optimized editor, VIM, Visual Studio Code, or whatever note taking app comes built into Mac). A C "compiler" would not expect many characters from Word so it would not be compatible easily with the C compiler. Some compiler include gcc and gnu. (These were not explained). Installing them is complicated and I have tried installing both GCC and GNU while using VSCode but whatever. Terminal window for programs is a bizarre thing and through a Mac is worse. Search for a free coding editor, VScode is great for beginning and even seasoned people use it (the free version). 

Would recommend writing on paper as well, at least to think through a program issue. 

The main loop for programming in C goes from Compiling, getting syntax editors, recompiling, running, getting a **wrong answer**, recompile, get a **correct** output, done which gives you a a.out file ("a" would be the name of the file I assume), which is like machine code that can "execute" (run a program using the memory of a computer and its C/G/TPU. I highlighted those words because I learned from a Software Testing course that programs are not just right and wrong, it isn't that black and white. 

One thing I can actually takeaway from these lessons is to get familiar with terminal commands, whether it is using Bash, or Unix, or Shell, etc., it helps when programming or doing any system commands to get more information on folders and files.

(Does programming directly on a terminal have less of a metadata trail? Why use a terminal to write code?)

---

Module 1 video 2 Debugging

Purposefully write code that will return an error, by return I mean it will break/not work and the computer will not be able to create a file executable of the program.  Program required 3 inputs to be given but only 2 were. The next error was an expression error of a missing character. Another bug demonstrated was using the number 0, because that always messes things up. 

---

Module 1 lecture 3 Finding the area of a circle

First introduced to the concept of input output and other elements of writing a C program. 

(Whoever uses white screen backgrounds for their editor should really consider the impact it has on other people.) 

We get a bunch of information given in a manner that does not explain anything. 

Introduces the word pre-processor token which means nothing to me as well as the PI convention used for "obvious reasons". Sure, pi is obvious enough, but if it is obvious enough we should know that it is an imaginary number that goes to infinity not (3.14159). Why call a program "main"? 

Identifiers are ordinary words but also keywords??
Initialize means what exactly?
Use printf("") to get a person's input into the program

What is an ampersand?
Parameter? Pointer? Memory? Address?

C doesn't do simplified operations like * 2 for a number to the power of, so its forces the use of repeated words.

return 0 does what exactly? Why?

---
Module 1 video 4

A little history lesson on C. Developed by Dennis Richie working at Bell Labs in 1972 and  had used 29 keywords and near machine code which allows for faster efficiency. Used to be called a Systems Implementations Language (SIL). Preceded by B, and Algol 60. Algol 60 is recommended to be studied as it is base to C which is base to many languages. 

We get the Hello World program in C. The use of main, keyword for data type identifier, printf to interact with a "user", curly braces, quotes, semicolons which signal the end of a statement. 

---

Module 1 video 5 (not really lecture when they are 2-10 minutes short)

Code should be readable so we have comments, thanks to the people who really began programming and had the vision/necessity to use collaboration on "projects". In C, comments are written between a /* and a * / 

An include <stdio.h> is called a pre-processor, a pre-processor is something that happens before the code/program written is "compiled". WTH is compiler. (I am familiar with the concepts of a compiler, interpreter, assembler, etc., since I studied Python and also looked into C++ so far). [Language Processors Explained | Baeldung on Computer Science](https://www.baeldung.com/cs/assembler-compiler-interpreter) , [Difference Between Compiler, Interpreter, and Assembler - Scaler Topics](https://www.scaler.com/topics/difference-between-compiler-interpreter-and-assembler/) (ad is a bit annoying on the latter site). What kind of definition necessitates more definitions?

Using stdio.h allows the program to use printf or else it would be "undeclared". Again, what is "undeclared"? (The only reason I emphasize these questions while going through the lessons is to highlight the curse of knowledge people seem to be ignorant about. Keeping things simple is always best. Sure another course more focused on presenting the inner workings of a language processor may serve this purpose better but this is a course and as such should aim to be most simple- any more than is necessary of course.)

---

Module 1 video 6

Another program example is used. A unit converter is used, mainly because the math involved is simple enough. Talks about the importance of matching characters like the curly brace specifically. Emphasizes the importance of proper identifiers which are names we give to things we assign values or operations to. instead of saying m = 345 we should write miles = 345 because it is important to readability. Some simple arithmetic operators are used. $$ 1.5033 * (miles + yards / 1240.02);$$
Numbers I used are arbitrary*

---

Module 1 video 7- audio was terrible

Showed examples of simple input and output using a temperature converter whereby a "user" provides what temperature to convert from Farenheit to Celsius.
# Core-Code Readme Week 1
READ ME for Core Code from scrath exercises ✌🏻

## 1. Interpreted and Compiled programming languages 
### What is a compiled programming language?
Compiled languages are converted into a binary language that the computer can understand and execute. This languages tend to be faster and efficient than interpreted languages, also, give more control over hardware aspects, like memory management adn cpu usage to the developer.

Some examples of compiled languages are C, C++, Rust, and Go.

### What is a interpreted language?
Interpreters run through a program line by line and execute each command. This languages are slower than compiled languages. but, with the development of **just-in-time compilation** that gap is shrinking. An advantage of this languages, is that are multiplataform, because they dont need that OS compile or create a new archive for the OS.

Some examples of interpreted languages, are JavaScript, Python, PHP.

## 2. Is Java compiled or interpreted, or both?
Java use a two-step compilation process. Java source code is compiled down to bytecode by the Java compiler. The bytecode ys executed by a Java Virtual Machine (JVM). Modern JVMs use a technique called **Just-In-Time (JIT) Compilation** to compule the bytecode to native instructions understood by hardware CPU on the fly at runtime.

## 3. Pseudocode currency converter 
### Description
You have been selected to develop the algorithm that will be used to convert dollars (USD) to bitcoin (BTC), for this the first thing you must do is deliver a pseudocode with the algorithm to be developed, in this way you can explain in a better way to the team what will be the required operation. The main idea is to have a website where the user will be asked to enter the amount to convert.

### Solution
1. START
2. Ask for the amount to convert to the user
3. Save the amount into a variable called A
4. A <-- amount that the user typed
5. Bit <-- bitcoin price
6. Result <-- A * Bit
7. PRINT "USD " + A + " = " + "BTC " + Result  
8. END

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

## 4. Your date of birth in the matrix?
### Description
Your team has just seen the movie "Matrix" and you have been asked, how the number of your year of birth would be written in binary. You must learn how to translate your date of birth into binary and show your team. (Do not use a webpage or a tool to convert your date of birth)

### Solution
1. START
2. 

## 5. MIPS exercises
### a. Create a program that adds any two given numbers provided by the user
Solution:

    .data
	            number1: .asciiz "\nType the first number: "
              number2: .asciiz "\nType the second number: "
              result_message: .asciiz "\nResult: "
    .text
	        main:
              li $v0, 4
              la $a0, number1
              syscall

              li $v0, 5
              syscall

              move $t0, $v0

              li $v0, 4
              la $a0, number2
              syscall

              li $v0, 5
              syscall

              move $t1, $v0

              li $v0, 1
              move $a0, $t0
              syscall
              
              add $t2, $t0, $t1 
              
              li $v0, 4
              la $a0 result_message
              syscall
              
              li $v0, 1
              move $a0, $t2
              syscall
              
### b. Create a program that displays your name
    .data
        name: .asciiz "\nFernando\n"
    .text
        main:
              li $v0, 4
              la $a0, name
              syscall
	      
## 6. Print special numbers
### Description
In this exercise you must use an iterative flow control to be able to print all the even numbers in the range of numbers from 0 to 100. Remember that you should not print each number, you should use a flow control structure to perform the exercise

### Solution
``` JavaScript
for(var i=0; i<=100; i++){
	if(i%2==0){
		console.log(i);
	}
}

```
## 7. Bad Code
### Description
The code shown below is not working in the right way, as a task you must find the error made by the developer who programmed this code and correct it, for this exercise you must explain what the error is and place the correct code

``` JavaScript
var cond = false;

if ((cond = true)) {
  console.log('The cond variable is true');
} else {
  console.log('The cond variable is false');
}
```
### Solution

```JavaScript
var cond = false;

if(cond){
  console.log('The cond variable is true');	
}else{
  console.log('The cond variable is false');
}

```

### Code's bug
The bug on this code, it was that the **cond** variable, was asigned as true on the if statement, for compare values its used **==**, or in this case my solution was only type the variable's name, cause an if statement compares as true in the condition.

## 8. Bad Code 2
### Description
You must create the code that follows the following logic, if the given number is 100, take this number as special and show the following message: "This is a special number!", but if the number is less than 1000, multiple of 10 and different from 100, you must show the following message: "This number is almost special". if none of the given conditions are met show the following message: "Just a regular number". Another developer was trying to program the logic, but apparently couldn't, you need to fix the code to work properly
```JavaScript
var n = 100;

if (n == 100) {
  console.log('This is a special number!');
}
if (n < 1000) {
  console.log('');
} else {
  console.log('Just a regular number');
}
if (n % 10 == 0) {
  console.log('This number is multiple of 10');
}
```

### Solution
``` JavaScript
var n = 100;

if (n == 100) { // if n equals 100, print 'This is a special number'
  console.log('This is a special number!');
}else if ((n<1000)&&(n%10==0)&&(n!=100)) { //if n less than 1000, and n is a multiple of 10, and different from 100, print 'This number is almos special'
  console.log('This number is almost special');
} else { // in other case, just print 'Just a regular number'
  console.log('Just a regular number');
}
```

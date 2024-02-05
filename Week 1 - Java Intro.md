---
title: Week 1 - Java Intro
attachments: [translation graph.png]
tags: [COMP 248]
created: 2024-01-17T15:21:16.367Z
modified: 2024-01-24T15:48:20.955Z
---

# Week 1 - Java Intro

### Sorting exercise morals
- **algorithm**
	- This is what we're focusing on in the class!
- efficiency
	- resources, in cs:
		- space (size)
		- speed (time)

Don't work on algorithm & syntax at the same time
Even a computer isn't *truly* multitasking, CPU always doing one calculation at a time

### End of lesson obj.
- Define and write an algorithm
- How is Java diff. from other OOP lang.?
- "Golden Rule"
- Locate main comp. of Java program
- Describe 3 types of errors

### Why program?
**Natural language**
- large vocab.
- complex syntax
- semantic ambiguity ✨

**Binary code/machine language**
- small vocab. (1s, 0s)
- simple syntax
- no semantic ambiguity 😔

Complete opposites!!! 🍎 vs. 🍊

**Programming language**
- bridges gap! guau ✨
- restricted vocab.
- restricted syntax
- nearly no semantic ambiguity


# General info

## Definitions
**Algorithm** <- focus of class
Step-by step process for solving problem, expressed in a natural language

**Pseudocode**
Algorithm expressed in more formal language, code-like, but does not follow a specific syntax

**Program**
Algorithm _expressed_ in a programming language, follows a specific syntax 

**Syntax**
Defines how we put together symbols, reserved words, and identifiers to make a valid program

**Semantics**
Defines what a statement means

## Golden rule
- Understand the problem
	- What is the problem?
	- What are the **inputs & outputs**?
- Design a solution (_algorithm_)
	- What are the steps?
	- Each step should be a **verb**
- Implement the solution (_program_)
- Test the program, refine

### Algorithm example
Write a program to find avg. of 3 days of temps.

**What is the problem?**
- Data input
	- 3 days' of temperatures
- Data output
	- Average of 3 days

**Design a solution**
- Get 3 temperatures
- Read 3 temperatures
- Calculate sum = t1 + t2 + t3
- Calculate avg = sum/3
- Display avg (on the console)

## Errors
3 main types

### Compile-time (syntax) errors
- Compiler will find syntax errors, other basic problems
	- Compiler will output "compile error",
		- Syntax
		- Rule
- Executable will not be created

### Run-time error
- Problem occurs during program execution, on CPU
	- Often mathematical
		- ex. divide by 0, log of neg. num., etc.
- Program will terminate abnormally

### Logical (semantic) error
- AKA bug
- Mistake in algorithm, our fault
- Compiler can't catch this
- Program will run, unexpected result

### Debugging
Process of eliminating bugs

"Bug" comes from Grace Hopper
Old computers, sometimes actual real bugs would interfere 🐛

# Java

## Basic info
James Gosling, Sun Microsystems 1991
Designed for home appliances
introduced in 1995

**OOP**
- Objects don't have single data element
- ex. car: red, speed, power, etc.
- originally, data component, now object

## Compiler
**Def**: software tool that translates source code into other language

Usually
- C, C++
- translates into machine language
- diff. types of CPU use diff. machine languages
- executable files don't work across platforms
- needs to be re-compiled for diff. platforms



### Java translation

**Java Compiler**
- Source code -> **byte-code**
- Machine language for Java VM
	- Thus, byte-code is very **portable** , works on any CPU
	- Is a bit slower

**Java Interpreter**
- Executes Java VM
- Translates byte-code into local machine language
- byte code -> machine code
	- relatively easy compared to initial compilation

![Java translation graph](@attachment/translation%20graph.png)

## Java program structure

	----------------Program------------------
	  --------------Classes----------------
	    ------------Methods--------------
	      ---Statements/Instructions---

Java programs always contain methods called *main*
- key to open door
- First method to run (?)
- Java compiler always looks for main
- only 1

Class name matches file name

Every statement needs a ";"

### Structure example

	//	comments on the program (authors, purpose, etc.)

	public class MyProgram // Class header
	{ // class body

		//	comments on the main method

		public static void main (string[] args) // method header
		{ // method body

			// declarations of variables and constants
			// statements of main method

		}
	}


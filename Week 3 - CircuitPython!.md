---
title: Week 3 - CircuitPython!
tags: [CART 346]
created: 2024-09-19T23:07:02.231Z
modified: 2024-09-20T00:11:01.690Z
---

# Week 3 - CircuitPython!

CircuitPython is a superset of Python 3
It's designed to simplify experimentation and learning to program on microcontrollers
Slightly higher level abstraction forked from MicroPython

Python is higher-level
easier to read, write (no semicolons, etc.)
indentation is important tho!
Built-in interpreter
open source!

Tricky thing: easy to want to be clever
Tempting to be terse, efficient, etc. in ur programs
*not* the point here
We want to understand what we're doing well,
let's start out more verbose

Easy to start, let's practice outside of class!

Most of our code won't be Python idiomatic code (not true Python code)
C++ style code in Python
A purist might turn up their nose

Dynamic variables!
Duck typing (looks like a duck, quacks like a duck, it's a duck)
Variables are objects!

burn into my mind: print() function!

logic operators are written out in Python!
and, or, not

Python has elif!

Preferably using functions instead of objects
More secure to not pass references

type() can be used to find out data type of an object
Sets v lists
no duplicates in a set!

## Digital v analog
Digital signals are discrete signals
Either 0V or 5V

When using digital io, we need to
- Tell Pi what pin we're using
- What direction the data is flowing in
	- Either input or output
- Set a default state

Analog signals are used to represent real-world pheonmena
They are continuous signals
No abrupt changes

ADC - Input
	- Analog to Digital Converter
	- Pi will discretize analog signal
	- Will give us discrete numbers
PWM - Output
	- Pulse Width Modulation
	- A digital signal cycled on and off so fast it produces an analog-like signal
	- modulating the duty cycle is what allows us to do so

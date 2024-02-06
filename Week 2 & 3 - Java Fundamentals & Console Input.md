---
title: Week 2 & 3 - Java Fundamentals & Console Input
tags: [COMP 248]
created: 2024-01-24T15:41:37.120Z
modified: 2024-02-06T02:49:11.458Z
---

# Week 2 & 3 - Java Fundamentals & Console Input

## Syntax & Conventions

### Comments

#### 3 types in Java
```
- // comment runs to the end of the line
- /* 
	this comment runs to the terminating
  symbol, across line breaks 
	*/ 
- /** javadoc comment */
	- ???
```

### Identifiers
Words a programmer uses in a program to name variables, classes, methods, etc.

#### Rules
- can contain 🟢
	- letters
	- numbers
	- _ (I've been working as a bank teller / For like eleven years...)
	- $ (dollar sign)
		- not recommended, can be confusing
- can not 🔴
	- begin with a number
	- be a reserved word
- no length limit
- case sensitive

#### Conventions
- Class names
	- Title case
	- Ex. MyClass, Bourgeoisie
- Constants
	- Upper case
	- LIGHTSPEED
- Variables, methods, etc.
	- Start with lowercase ()
	- Ex. aVar, a_va

#### Predefined identifiers!
Can technically be redefined, can be confusing and dangerous
```
Keywords:

abstract  continue  for         new        switch
assert    default   goto        package    synchronized
boolean   do        if          private    this
break     double    implements  protected  throw
byte      else      import      public     throws
case      enum      instanceof  return     transient
catch     extends   int         short      try
char      final     interface   static     void
class     finally   long        strictfp   volatile
const     float     native      super      while
```

### Indentation
- Spaces, blank lines, tabs, - white space
- Used to separate words and symbols in a program
- Extra white space ignored by compiler

Curly brackets on own lines
Stuff goes inside

## Primitive Data Types
User manipulated data

### Numeric

#### Integers
4 types (keywords), different sizes, amount of bytes
- byte
	- 1 byte
- short
	- 2 bytes
- int
	- 4 bytes
- long
	- 8 bytes

We will generally be using "int"s in the class

#### Floating point numbers
2 types (keywords), different sizes
- float
	- 4 bytes
- double 
	- 8 bytes

Floating-point numbers aren't precise, as there is a limit to how many digits after the decimal point can be represented

### Characters
Single characters
- keyword char
	- 2 bytes
	- Any unicode character
- Deliminated by single quotes
- Ordered according to a character set
	- ????
- Corresponds to unique number code
	- Unicode character set
		- ASCII: smaller subset of unicode

### Boolean
True or false
reserved words true and false only valid values
*Not* 0 & 1

## Variables

**Def**: Name for a location in memory, used to store information

### Declaring
Must be declared before it is used
- Indicate variables

```
// data type | Variable name
	        int total;
```

Multiple variables can be created in one declaration

	int count, temp, result;

### Initializing
Variables can be initialised in the declaration

	int sum = 0, speed = 1;

Uninitialized variables are given default values, although it's bad for readability to depend on these
- int
	- zero
	- 0
- long
	- zero
	- 0L
- float
	- positive zero
	- 0.0f
- double
	- positive zero
	- 0.0d
- char
	- null character
	- \u0000
- boolean
	- false

## Constants
Similar to variables, but only hold one value while program is active. The compiler will throw an error if you try to change the value

Declare a constant using the **final** modifier, followed by data type:

	final int MIN_AGE - 20;

Uses
- give names to otherwise unclear literal values
- Facilitates updates of values used throughout program
- Prevent accidentally changing a value

## Java standard class library
Collection of classes that we can use when developing programs
Organised into packages

### Import declaration
Can import either the entire class, or just a single class

	import java.text;

	import java.text.DecimalFormat;

note: java.lang automatically imported into all programs

### Console input
Uses the Scanner class
Keyboard is represented by the System.in object

	import java.util.Scanner;

	Scanner myKeyboard = new Scanner(System.in)

### Input - Reading primitive data types from a scanner
uses next*Something*() method
- nextBoolean(),
- nextByte(),
- nextInt(),
- next() (strings)
- etc.
```
Scanner myKeyboard = new Scanner(System.in);
System.out.printIn("Your name:");
String name = myKeyboard.next();
System.out.PrintIn("Welcome" + name + " Enter your age:");
int age = myKeyboard.nextInt();
```

This interaction occurs in the console
next() makes the program wait for user to press enter
I can ask for multiple inputs one after the other and spaces are read as breaks from one call to the other

Once done, Scanner.close() should be called
Could run without it(?) but Java won't be happy, for security purposes

## Output
- System.out.print() 
	- Displays what is in parenthesis
- System.out.println()
	- Displays what is in parenthesis & advances to the next line

### Multiple output 
#### (+ in output)
Inside print() & println(), + executes a concatenation
If inside parentheses inside print(), it will execute an addition

```
int x = 1, y = 2;
System.out.println("x+y="+x+y); // Outputs x+y=12
System.out.println("x+y"+(x+y)); // Outputs x+y=3
```

*Not* dependant on data type, but syntactic context
This only applies to +, as it is the only one that doesn't have a purely arithmetic function

#### Multiple lines
Strings can not be cut over multiple lines
Will lead to error

### Escape sequences

``` 
System.out.println("He said "hi" to her"); 
```

Would result in an error, as " is used for delineating strings

Thus, one can use \
- Applies only to next character
- Allows to print characters such as "

The following would work:

``` 
System.out.println("He said \"hi\" to her"); 
```

List of escape sequences
- \b
	- prints backspace
- \t
	- prints backspace
- \n
	- prints to new line
- \\"
	- prints double quote
- \\'
	- prints single quote
- \\\
	- prints backslash


## Assignment
### Def: 
Used to change the value of a variable
The assignment operator is '='
_Syntax_: Variable = Expression

Semantics:
The _expression_ on the right is evaluated
The result is stored in the variable on the left (overwriting any previous value)

### Extra assignment operators
- **+=**
	- Ex. x += y
	- is x = x + y
	- Can also do string concatenation
- **-=**
	- Ex. x -= y
	- is x = x - y
- ***=**
	- etc.
- **/=**
- **%=**


### real division
With floating point numbers
Returns a decimal number

### integer division
both operands are integers, returns just an integer, 
ie 10/8 == 1, 8/10 == 0

### Operator precedence
Operators can be combined into complex expressions

**Precedence**
1. Casting
2. Parenthesis
3. _Unary_ + & -
	- Needs only one operand
	- ex. ++ and -- ???
4. Multiplication, division, and remainder
5. Addition, subtraction, and string concatenation
6. Assignment operator

### Operator associativity

#### Unary operators
Operators of equal precedence are grouped **right-to-left**
Ex. +-+rate is evaluated as +(-(+rate))

#### Binary operators
Operators of equal precedence are grouped **left-to-right**
Ex. base + rate + hours would be evaluated as (base + rate) + hours

#### Assignment operators
A string of assignment operators is grouped right-to-left
n1 = n2 = n3 would be evaluated as as n1 = n3

### Increment and decrement operators
ie ++ & --
Unary operators!

#### Prefix form
- Value is inc./dec. by 1
- The value of the entire expression uses the **new** value of the variable (after the inc./dec.)

#### Postfix form
- Value also inc./dec./ by 1
- The value of the entire expression uses the **old** value of the variable (before inc./dec.)

#### Examples
```
int nb = 50;  int nb = 50;  int nb = 50;    int nb = 50
++nb;					nb++;					int x;					int x;
                            x = ++nb;				x = nb++;

nb: 51        nb: 51        nb: 51, x: 51   nb: 51, x: 50

int nb = 50;			int nb = 50;			int nb = 50;			int nb = 50;
int x;						int x;						int x;						int x;
x = ++nb + nb;		x = nb++ + nb;		x = nb + ++nb;		x = nb + nb++;

nb: 51, x: 102		nb: 51, x: 101		nb: 51, x: 101		nb: 51, x: 100
```

## Assignment compatibility
Java does not generally allow for operations between multiple types

There are 3 ways to convert types:

### Arithmetic promotion


### Assignment conversions
Occurs when an expression of one type us assigned to a variable of another type

This only happens if variable is of a wider type than the expression, expression is widened (once it's completed!)

#### ex. 
- long = int
- double = int
- etc.

#### Limitations
- Boolean are not compatible with any other type
- Narrowing conversion will not work, ie assigning a wider type to a narrower type
	- ex. int = double

### Casting
Type conversion can be forced:
**Syntax**: (desired_type)expression_to_convert

Ex.
```
int aVar = (int)3.7
// aVar: 3
// (note! will round down going from floating point to integer)

byte b1 = 1, b2 = 127, b3;
b3 = b1 + b2; // ❌
// When b1 & b2 are added, they are converted to int's
// Thus, u end up trying to assign an int to a byte, which is a narrowing assignment
// Instead, you should do the following:
b3 = (byte)(b1 + b2)
```

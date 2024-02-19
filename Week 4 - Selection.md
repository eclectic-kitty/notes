---
title: Week 4 - Selection
tags: [COMP 248]
created: 2024-01-31T15:23:10.823Z
modified: 2024-02-14T16:26:18.377Z
---

# Week 4 - Selection

## Flow of control
1. **Sequence**
	- Unless specified otherwise, the order of statement execution is linear/sequential
	- One statement after the other, in sequence
2. **Conditional statements**
	- A statement may or may not be executed, depending on some condition
3. **Repetition statements** 
	- A statement is executed over and over, repetetively, until some condition becomes true or false

Latter two are decisions based on Boolean expressions (conditions)

### Flowchart
A graphica way of representing an algorithm
ie another form of pseudocode

*insert image from slides here*

## Conditional statements
Java has 3:
1. **if** statement
2. **if-else** statement
3.  **switch** statement

### If & else statements
	if(condition) {
		statement;
	} else {
		statement2;
	}

"if" being a reserved word
"condition" being a boolean expression

Note: if statements can work without curly brackets
In this case, only the next statement after the if statement will run

#### Dangling else
Else's are always matched to the last (unmatched) _if_ statement
ex.

	if (condition1)
		if (condition2)
			statement1;
	else
		statement2;

this else will match to the inner _if_, if not otherwise specified

	if (condition1) {
		if (condition2) {
			statement1;
		}	
	}
	else 
		statement2;

Now, it will match to the outer _if_

### Switch statement
Used instead of a whole bunch of nested _if else if_'s

#### Syntax
_switch_ will compare the expression to the *valuen*'s and run the statement inside if it matches

	switch ( expression )
	{
		case value1 :
			statement-list1;
			break;
		case value2 :
			statement-list2;
			break;
		case value3 :
			statement-list3;
			break;
		default:
			default-statement-list;
	}

_break_ and _default_ are optional

#### break
This will cause control to be transferred to the end of the switch
If it isn't used, the flow of control will continue into the next case, regardless of whether expression matches that case's value

#### default
This case will run in case none of the other cases match

### Conditional operator *?*
Shortcut to an if in some cases
Ternary operator

Syntax:

	condition ? expression1 : expression2
Semantics: If the condition is true, expression 1 is evaluated, if it is false, expression 2 is evaluated

ex.

	larger = (num1 > num2) ? num1 : num2;
	System.out.println(larger);

Look into parentheses more

ex. 2

	System.out.println("Change is " + count + ((count==1) ? " Dime" : " Dimes"))

How many of these parentheses do we need in this example?

### Comparisons

#### Symbols
- ==
- !=
- >
- <
- =>
- =<

#### Note on floats!
Don't use == with floating point numbers!
Floating point numbers are approximated
Represented weirdly on the machine
Instead, use < or >, as we only want to see if they are *close enough*

#### Characters
Relational operators can be used with characters!
a < b is true because the unicode value of a is smaller than that of b

#### Strings
Relational operators can not be used with strings, as they are objects
Instead, strings have the equals() method.



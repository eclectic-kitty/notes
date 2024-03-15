---
title: Tutorials
tags: [COMP 248]
created: 2024-03-10T01:02:53.017Z
modified: 2024-03-10T06:17:06.718Z
---

# Tutorials

## Tutorial 2

### Q1
integer, double, character, string

### Q2
Greetings, g, (\<greeting\>?)
yass, yass, **nein, only the special characters _ and $ are ok**

### Q3
5
5 - oops! gets saved as double, so 5.0
3
3 - same, 3.0
3.something
1.something
0
2
6

### Q4
A. 
result: 3+4
result: 7 (or 34, think it might be the latter) - **I caught myself! it's 34 cuz of order of operations)**
result: 34
result: 7

B.
```
System.out.print("The file is in c:\\Temp\\theFile.txt");
```
Admittedly not sure if **the double slashes are needed**
I was correct! They were needed!

C.
John

## Tutorial 3

### Q1
a) 5

b) 6

### Q2
- 21
- 3
- -20
- 30 < 30 || 13 > 12
	- false || true
	- true
- true || false && true
	- true || false
	- true

### Q3

x = 10
y = 4
iresult = 1
w = 4.5
z = 8.2
fresult = 8.2/2 = 4.1

```
iresult now is: 1
fresult now is: 120.0

fresult now is 4.1

fresult now is 2.0
fresult now is 2.5
```

### Q4
A. 
quest for the zoly grail Quest for the zoly Grail

B.
10, 9

C.
a. Agent5
b. Agent5 **(can u do += for concatenation?) - the answer is yes!**

D.
- a. " Here"
- b. "our N"
- c. "our Name Here" - Oops! **The second parameter of String.substring() is exclusive**, so there's no e
- d. 14
- e. 3
- f. n/a - Apparently String.indexOf() returns -1 if the string or character never occurs

### Q5
```
The line of text to be changed is: 
I hate programming.
I have rephrased the line to read:
I love programming.
```

## Tutorial 4

### Q1
```
The condition evaluated to true!
```

### Q2
```
The condition evaluated to false!
```

### Q3
```
if (weight < 116)
	You're fine!
else if (weight <= 130)
	You're fine!
else if (weight <= 200)
	You're fine!
else
	You're fine!
```

### Q4
```
if (preTotal <= 20.0)
	shipCost = 5.99
else if (preTotal <= 65.0)
	shipCost = 10.99
else
	shipCost = 15.99
```

Would it complain about a double being compared with an int?

Apparently it **wouldn't complain about comparing a double and an integer**

### Q5
true
true
false
true

### Q6
```
Under the limit
Under
Over the limit
```

### Q7
- true - Bruh, _false_, because 5 > 6 is false
- true - **investigate** I thot the right side would be false, but **app. if the right side of a % expression is larger than the left side, it returns the left side**
- syntax error, a single | is not an operator
- false
- false ? **not sure if u can double '!' - you can!**
- syntax error, I feel like it would evaluate the first part to be true and then it wouldn't like true being an operand in a comparison - A similar valid thing would be: (0 <= x && x <= 10)
- syntax error, strings can't be operands for comparisons
- No syntax error, but initial would become Y
- false

### Q8
**Didn't have time!**

## Tutorial 5

### Q1
See T4, Q3

### Q2
See T4, Q4

### Q3
a)
```
case 1
15 11 100

b)
default
0 10 100

c)
case 2
default
0 2 100
```

### Q4
```
if (age < 10)
	rebate = 20;
else if (age > 70)
	rebate = 20;
else if ( age < 20 && isAStudent && workExperience > 4)
	rebate = 15;
```

**Oops! under 10s and over 70s get the same rebate, so that could've been** 
```
if (age < 10 || age > 70)
	rebate = 20;
```

## Tutorial 6

### Q1
A.
```
0 2 4 6
```

B.
```
7 6 5 4
```

C.
```
1 1*
1 3*
2 1-
2 3-
3 1*
...
5 3*
```

**Wrong** 
```
1 1*1 3*
2 1-2 3-
3 1*3 3*
4 1-4 3-
```
**Watch out for tricky bad indentation! The println(); was *outside* the inner for loop**

D.
```
while 30 3
while 10 4
while 9 3
the end 3 4
```

E.
i = 1
count = 5
```
0 5
1 16
2 8
3 4
4 2
```

F.
**Didn't do**

G.
**Didn't do**

H.
```
Hello
Hello
Hello
...
```
**Wrong!** There is no output! There was a sneaky ';' after the while's condition, causing it to never run

### Q2
```
count = 2;
do {
System.out.println(count);
count += 2;
} while (count <= 10)
```

**Oops! Forgot to initialize count**
**Also, do ... while loops need a ';' after the condition!**

### Q3
```
count = 2;
while (count <= 10) {
System.out.println(count)
count += 2;
}
```

**Oops! forgot to initialize count**

### Q4
**Didn't do!**

### Q5
**Didn't do!**

## Tutorial 7

### Q1
A.
This either won't work because of incrementing during check, or
```
2
3
```
**oops** careful! it was print(), not println()
**also, it does work app.!**

B.
```
1
2
3
```

C.
```
for (int i = 1; i++ < 4;)
```
Same as A.
**Wrong! i++ means it passes the < 4 check while incrementing, thus being incremented for the print()**
```
234
```

D.
Same as B.

E.
ch = K
```
0BEHKN
1BFJN
2BGL
```

F.
```
Not multiple...
3
5
End
```

H.
k = 7
j = 1
sum = 42
```
 7+ 5+ 3+
 6+ 4+ 2+
 5+ 3+ 1+
 4+ 2+ 0+
 3+ 1+ -1+
 2+ 0+ -2+
 1+ -1+ -3+
 = 42
```
**wrong** but also why would this be a question
anyway, watch out for **non-constants in for loop conditions**
### Q2

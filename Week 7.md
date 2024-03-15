---
title: Week 7
tags: [COMP 248]
created: 2024-03-06T15:35:20.929Z
modified: 2024-03-08T16:07:50.855Z
---

# Week 7

## Sorting theory
Process of arranging a list of items in a particular order

Examples:
- Selection sort
- Insertion sort
- Bubble sort
- Quicksort

### Selection sort
Select a value and put it in its final place into the list. Repeat for all values

Algorithm:
- Find the smallest value in the arry
- Switch it with the value in the first position
- Find the next smallest value
- Repeat until end

## Multidimensional arrays
An array containing (references to) separate arrays
Can be thought of as a table

Important distinction: 
The outer array does not contain the data itself of the inner arrays
The outer array only stores **references** to the inner arrays

## Multidimensional arrays
### length
length variable contains only length of one of the dimensions
ex.
``` 
char[][] page = new char[30][100]
page.length // contains 30
page[0].length // contains 100
```

 0  1  2 ... 9
10 11  ...  19
20    ...   29
     ...
40    ...   49

### Ragged arrays
An array where the second dimension is of different lengths

```
double[][] a = new double[3][5];
same as
double[][] a;
a = new double[3][];
a[0] = new double[5];
a[1] = new double[5];
a[2] = new double[5];
```
Therefore, we can vary the lengths when declaring each section of the second dimension

```
double[][] a = new double[3][];
a[0] = new double[5];
a[1] = new double[10];
a[2] = new double[4];
```
Note, while the dimensions haven't been declared, the reference is to null

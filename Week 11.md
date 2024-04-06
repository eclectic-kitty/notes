---
title: Week 11
tags: [COMP 248]
created: 2024-04-03T15:06:47.361Z
modified: 2024-04-05T14:49:25.389Z
---

# Week 11

## Arrays

Arrays are objects!

When you define the reference, all you have is the reference
You have to create the object itself
```
Int[] nameOfArray;
nameOfArray = new Int[5];
```

### Arrays as parameters
When an array is passed as a aparameter to a method, what is passed is only the reference, not the array itself. The parameter and the original reference are aliases of each other

Thus, if you modify an element of the array inside the method, it changes outside as well

### Arrays and assignment
It is not possible to change the size of an array
But,
It is possible to assign an array's reference to another array

### Duplicating / Copying an array
In order to duplicate an array, one would need to 
	- Create a new array with same length as original
	- In a for loop, copy over the value at each index of the original

There is a built in clone() that does this though
The array it returns is a generic object though, has to be cast to the type we want
```
theCopy = (int[]) theOriginal.clone();
```

### Privacy leaks with array (or object) instance variables

An accessor method for an array attribute (or other objects) should not return the object directly, as instead of returning the value of the object, it will retunr a reference to the array directly.
```
public int[] getArray() {
	return anArray;
}
```
Instead, it should return a **deep copy** of the array.
```
public int[] getArray() {
	int[] temp = anArray.clone();
	return temp;
}
```

Note: this is not important for strings, as they are immutable.

## Arrays of objects
In an array of primitive types, the array stores the data itself
In an array of objects, what is stored is references to the objects, not the objects themselves

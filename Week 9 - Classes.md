---
title: Week 9 - Classes
tags: [COMP 248]
created: 2024-03-20T14:37:53.382Z
modified: 2024-03-20T15:08:03.640Z
---

# Week 9 - Classes


### Static
Static methods and attributes are shared across the entire class, ie all objects share the same version

To call outside of the class, the name of the class has to be called,
```
MyClass.method()
MyClass.attribute
```

### Non-static

## Methods

Two types of methods
- Methods that compute and return a value
- Methods that perform an action
	- Do not return a value
	- called a *void* method

### Methods that return a result
Similar to a math function
Must specify type of value in its heading
```
public typeReturned methodName(paramList)

Ex.:
public boolean isTail() {
	if (face == 1)
		return true
	else
		return false
}
```

#### Return statement
Allows the method to "return" a result back to the calling method

Syntax:
return expression;

What does it do?
1. The expression is evaluated
2. The value of the expression is returned as the result of the method
3. The method is exited

Types it can return
- primitives
- objects
	- strings
	- arrays
	- etc.

### Void methods
Methods that perform an action but do not *evaluate* to a value

Example uses:
- Displaying something
- Changing the value of an attribute
- etc.

They officially return **void**
*void* *has* to be present at the start
They use no *return expression*
*return;* to end method is optional

### Calling methods

Methods that return a result are expressions that have a type and value:
```
aVar = objectName.methodName();
System.out.print(objectName.methodName());
```

Methods that do not return a result are *not* expressions:
```
objectName.methodName();
```

---
title: Week 12
attachments: [Clipboard_2024-04-12-11-34-58.png, Clipboard_2024-04-12-11-35-04.png]
tags: [COMP 248]
created: 2024-04-12T14:52:22.017Z
modified: 2024-04-16T15:01:26.203Z
---

# Week 12

### Equality of references
The == operator can be used to compare equality of *references*.
Returns true if the references are aliases of each other, if both variables refer to the *same* object

### equals()
Unless redefined, equals() is the same as using the == operator,
i.e. will return true if the objects are the *same*

## Garbage collection
If an object no longer has any references, it can't be used anymore

Java has an automatic garbage collector
- Runs periodically
- Returns memory of inaccessible objects to the system for future use

If a reference is no longer useful,
- Assign it to null so that the garbage colelctor can pick it up

In some other languages, the programmer is responsible for performing garbage collection as automatic garbage collection uses up resources

## Argument passing

### By value
All primitive types are always passed by value

The formal parameter is a copy of the actual parameter
The method modifies the copy
The original/actual paramater is never modified

### By reference
Object parameters are always passed by reference

We are copying only the reference, not the object
The actual parameter and the formal parameter are aliases of each other
The method can modify the actual paramaters

### Wrapper classes for primitive types
Existing wrapper classes, when passed to a method, will still pass the value
- ex. Integer, Byte, Long, Double, etc.

## Anonymous objects

**new operator**
Calls a constructor which initializes an object
Returns a reference to the location in memory of the object created

If the object created will only be used as an argument to a method, never to be used again, there is no need to assign it to a variable
You can just create it and use it

```
BankAccount temp = new BankAccount("mary", 100);
if (someAccount.equals(temp))
	System.out.print("wahoo");

if (someAccount.equals(new bankAccount("mary", 100)))
	System.oout.print("wahoo");
```

## Attributes

### Private
Declaring an attribute as private is enough for primitive types,
but not for objects, as the only thing that's private is the object *reference*

### Avoiding privacy leaks

#### Constructors
Careful when accepting objects as parameters
The underlying object will be the same and the new object's attribute will merely reference to this underlying object
Thus, the private instance attribute will be accessible from outside of the class!

Instead, one must create a deep copy of the inputted parameter.

#### Setters/getters
Similarly to constructors, one has to make copies before passing or accepting object parameters!

### Immutable class:
A class that contains *no methods* (other than constructors) that *change* an object's *data*
**It's safe to return a reference to an immutable object!** because the object cannot be changed

**Example**: String!

### Mutable class:
A class that contains public methods that *can change* an object's *data*
Never write a method that returns a mutable object directly, always create copies.

## Exam:
30-40% midterm material
Rest is classes!

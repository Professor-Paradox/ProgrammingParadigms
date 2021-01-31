# Procedural Programming Paradigm  

Procedural Paradigm is the Most used Imperative paradigm.  
This is the easiest paradigm to learn.  
It is close to cpu architecture,we can learn how a compiler/interpreter/cpu works and think like one.  

With Procedural Programming we can created better core logic.  
This is also time consuming process as we have to worry about a lot of things while creating a logic so that it won't cause unexpected failures.  

languages implementing Procedural Paradigm are:  

1. [C](../C/C.md)
2. [C++](../C++/C++.md)
3. [C#](../Csharp/Csharp.md)
4. [Python](../Python/Python.md)

---

**Index**  

- [Procedural Programming Paradigm](#procedural-programming-paradigm)
  - [Program Structure/Syntax](#program-structuresyntax)
  - [Compilation/Execution](#compilationexecution)
  - [Keywords](#keywords)
  - [Identifiers(Naming Conventions)](#identifiersnaming-conventions)
  - [Variables/Data Types](#variablesdata-types)
    - [Data Types](#data-types)
    - [Scope](#scope)
    - [Global/Local Variables](#globallocal-variables)
    - [Stack Memory](#stack-memory)
  - [Operators](#operators)
    - [Arithmetic](#arithmetic)
    - [Relational](#relational)
    - [Logical](#logical)
    - [Other Operators](#other-operators)
  - [Control Flow Statements](#control-flow-statements)
    - [Iterative](#iterative)
      - [For/For-Each](#forfor-each)
      - [While/Do..While](#whiledowhile)
    - [Conditional](#conditional)
      - [If](#if)
      - [If..else If](#ifelse-if)
      - [If.. If](#if-if)
      - [Switch](#switch)
    - [Extra Control Flow Statements](#extra-control-flow-statements)
  - [Methods/Functions](#methodsfunctions)
    - [Parameterized Functions/Methods](#parameterized-functionsmethods)
    - [Variable Length Arguments](#variable-length-arguments)
    - [Method Overloading](#method-overloading)
  - [Input/Output](#inputoutput)
    - [Scan Input](#scan-input)
      - [From User](#from-user)
      - [From Files](#from-files)
    - [Give Output](#give-output)
      - [To User](#to-user)
      - [To Files](#to-files)
  - [Arrays/Strings](#arraysstrings)
    - [Arrays](#arrays)
      - [Creating Arrays](#creating-arrays)
      - [Using Arrays](#using-arrays)
      - [Built-in Array Methods/Functions](#built-in-array-methodsfunctions)
    - [Strings](#strings)
      - [Creating Strings](#creating-strings)
      - [Using Strings](#using-strings)
      - [Built-in String Methods/Functions](#built-in-string-methodsfunctions)
  - [Modularity](#modularity)
    - [Structure of Project](#structure-of-project)
    - [Splitting Relevant Logic](#splitting-relevant-logic)
    - [Reusing Existing CodeBase](#reusing-existing-codebase)



All these sections are created again in each of the programming language files for easy understanding and an example code is provided.  


## Program Structure/Syntax

Program Structure is the pattern in which we have to write our source code, this pattern should be followed for the execution to go smoothly.  
Depending on the language the structure changes.  

To remember it easily and for better interOperable code(code that is similar and easy to read irrespective of language) we write the most important, needed code at the start of program and the actual logic after it.  

**Ex:**  
```C
#include<stdio.h>
int x=5;// needed code for execution
int main(){
    printf(x);//actual logic
    return 0;
}
```


## Compilation/Execution  

Depending on the specific language the compilation and execution defers with different commands on different platforms.  
Here is an example:

```bash
gcc main.c #is used to execute c file in linux

javac main.java # is used to compile java file in any O.S

python main.py # is used to execute python file in any O.S
```

## Keywords

Keywords are the english words that are used during the development of the language.  
So the creators of that specific language, put certain restrictions on how to use these keywords.  
If we don't follow these rules the program won't execute.  

Think of this like this we give our dog and our friend the same nick name. In this case if we call our friend to bring some thing and our dog tries to understand it but gets confused. 

Same way all programming languages have certain meaningful words that have to used as guided.  

Example: 

```java
// these are java reserved keywords thats why they are highlighted in different ways
int float double 
main() this super

// these are normal english words without any default meaning to language 
hello name time location 
```

```c
// these are some keywords in c language
#include<stdio.h>
int float 
return 

// these are some english words in c with no significance 
hello name time location
```


## Identifiers(Naming Conventions)  

If we want to create a logic we need to name things. they can be data, functions etc.  
the only rule common to all languages in this guide is to **not use keywords** for naming.  

Each language has its own naming conventions.  
But in the IT industry we follow one convention that makes our codebase clean and easy to maintain, across multiple languages.  

These are conventions, not rules or guidelines and change depending on the company and project.  
The main purpose of Identifying something in our code is to make it easy for us to use it and modify it.  

Some popular conventions are 
1. **PascalCaseNotation** here we make all words first letter in our name capital case.
   - Some examples are T**hisIsMyName**, **WhatIsTheTime**, **HowLongThisTutorialWillLast**.
   - Most used by java.
2. **camelCaseNotation** Here we make all words except first words first letter Capital case.
   - Some examples are **thisIsMyName**, **whatIsTheTime**, **howLongThisTutorialWillLast**. 
3. **snake_case_notation** here we separate our words with an underscore.
   - Some examples are **this_is_my_name**, **what_is_the_time**, **how_long_this_tutorial_will_last**.

There are more conventions but we use all these conventions depending on our need and stick to it.  

## Variables/Data Types

In our programming logic we need to store data.  
At the beginning we will perform basic math programs.
So we need to store numerical values, depending on the language we can store directly(python) or we say which type of data we want to store then store it(java,c).  

Example
```java
int x=5;//here x is a variable and stores 5
```
```python
x=5; # here x stores 5 
```

### Data Types

Since we can store any thing from numbers to images to videos, we have to classify the types of data we can store.  

Irrespective of language these are the most common data types in all programming languages.  

1. **int** stores integer values
2. **float** stores decimal values
3. **double** stores decimal values with more precision
4. **char** stores characters
5. **boolean** stores either true/ false
6. **Strings** stores strings

There are even more data types, but each language supports different data types.  
Learn the specifics in the respective language guide.  

### Scope

Scope is the concept of visibility of a variable or method in a code file.  
Think of it as the real scope of gun, we can only kill that is with in our scope.  
Same goes for the Source Code scope.  

We can only access variables that are visible to current file/method.  
Depending on the language there are restrictions on what can access what.  

The scope of a method or file starts from open curly brace and close curly brace.  

```java
method(){
    int x=5;
}
//can't access x here since it is inside method, so out of scope.
```

Scope is divided into two types:
1. Local scope: the scope of a single method is called local scope.The data inside it can't be accessed out of that scope.
2. global scope: the scope of an entire program file is called global scope of that file. The variables in global scope can be accessed by any other local scope data.  

### Global/Local Variables

Data inside local scope is called local members(local variables+local methods)
Data inside global scope is called global members(global variables+global methods)


### Stack Memory

Stack memory follow first in first our approach and is used for storing global variable and to execute our code.  

## Operators

Operators are the operations that can be performed on two statements. 
Operators are divided into multiple categories. 
### Arithmetic

Arithmetic operators are used to perform math operations. 
addition(+),substraction(-),multiplication(*),division(/),reminder/modulus(%)
### Relational

Relational Operators are used to perform relational calculations. 
whether two statements are related are not 

equals(==),not equal(!=),less than(<),less than equal(<=),greater that(>),greater than equal(>=)

### Logical
logical operators are used to perform logical operations between two statements.

And(&&),or(||),not(!)

### Other Operators  
There are some more operators depending on the support provided by the language.  
Some of them are **?** in java for easy if operator


## Control Flow Statements

control flow statements are used to control our execution flow.  

### Iterative
iterative statements are used to perform some tasks repetitively.  


#### For/For-Each

#### While/Do..While

### Conditional

#### If

#### If..else If

#### If.. If

#### Switch  

### Extra Control Flow Statements

## Methods/Functions

### Parameterized Functions/Methods

### Variable Length Arguments

### Method Overloading

## Input/Output

### Scan Input

#### From User

#### From Files

### Give Output

#### To User

#### To Files

## Arrays/Strings

### Arrays

#### Creating Arrays

#### Using Arrays

#### Built-in Array Methods/Functions

### Strings

#### Creating Strings

#### Using Strings

#### Built-in String Methods/Functions

## Modularity

### Structure of Project

### Splitting Relevant Logic

### Reusing Existing CodeBase

Shadowing:  
Using Same Name for Local Global Variables is not preferred,but is allowed by languages.  
But when accessing the variable Compiler/Interpreter will use the first accessible variable,in its scope.  
This is called Shadowing of global variable.  
Since global variable is hidden due to presence of local variable.  

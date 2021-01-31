- [Introduction to Programming Languages](#introduction-to-programming-languages)
  - [Compilation vs Interpretation](#compilation-vs-interpretation)
    - [Compilation](#compilation)
    - [Interpretation](#interpretation)
- [Programming Paradigms](#programming-paradigms)
  - [Imperative Paradigm](#imperative-paradigm)
    - [Procedural Paradigm](#procedural-paradigm)
    - [Object Oriented Paradigm](#object-oriented-paradigm)
    - [Parallel Processing Paradigm](#parallel-processing-paradigm)
  - [Declarative Paradigm](#declarative-paradigm)
    - [Logical Paradigm](#logical-paradigm)
    - [Functional Paradigm](#functional-paradigm)
    - [Database Paradigm](#database-paradigm)
  - [Useful Documents](#useful-documents)

## Introduction to Programming Languages  

Computers are amazing machines that can play music, games, videos, or you know create applications that can send people to the moon and mars for fun and research.  

But computers Only Understand 0 and 1, either to turn on the gate(AND, OR, XOR, NOT, NAND, NOR) or turn off the gate to perform calculations.  

A Programming Language is just a Vocabulary and a set of instructions used to communicate with the machine(Computer) To perform a certain task.  

There are 4 Types of Programming Languages:

1. **Machine Language**  
    In World War 2, computers were mainly used/designed to crack encryption.  
    After the war, computers are used in industries, companies, institutions for Research and Education.  

    ![First computers the size of a board room](./../../img/MainFrame.jpg)  
    These **Mainframes** are used with plugboards, punch cards, analog switches to take instructions and perform a specific operation.  
    This was tedious, after the invention of the transistor, binary code replaced analog programming.  

    Instructions are given to Computer in binary(0,1) format and different sequence of 0,1 meant different things,It was **possible** but turned to a nightmare(for users/programmers) real quick.  

    Ex:`2+3=5`, is performed using 0's and 1's, like this.`010+011=101` in binary.  
    If Just addition is this complex, imagine instructing a Computer to Perform Complex Trigonometric or Theoretical Math Equations, it was a nightmare.  

    Ex: To calculate a Trigonometric equation it would take an hour to code it in binary. (0's 1's as code).  

    ![Machine Code Example](./../../img/MachineCode.png)  

2. **Assembly Language**  
    Computer Scientists got tired of writing equations and instructions to computers in binary, so after some time and research Computer Scientists created **Assemblers**.  

    Assemblers contain binary code with higher abstraction, with this we can just write a single line of code that gets converted to the respective binary code.  

    Ex: add a b(will be replaced by the assembler to about 30 lines of binary code, that the machine can understand and compute)  
    For a time this was easier than binary coding(machine coding), many languages that used this philosophy are called **Assembly languages**, they all had an assembler built for this use.  

    Even this approach faded out quickly as the need for complex operations grew, like calculating trajectories of missiles, cannonballs, planes, etc.  
    These operations **can** be performed with Assembly Languages but are not easy to write and modify.  

    Higher-level computations were tough with assembly level programming. New programming languages like C, Fortran, COBOL gave better abstraction.  
    Since we are writing our equations and instructions in assembly it is CPU/Device Specific and any change of device, Assembler version, CPU would need a full code to rebase.  
    ![Assembly Language Example](./../../img/AssemblyCode.png)  

3. **Medium-level Language**  
    Medium Level Language is an abstraction to Assembly Language and is not used by Programmers rather by High-level Languages.  
    C Intermediate Code and Java Byte code are examples of Medium Level Languages.  
    This code is optimized for a specific Device/CPU/Architecture, for execution.  
    ![Medium level byte code example](./../../img/ByteCode.png)  
4. **High-level Language**  
    High-Level Languages are Abstraction to Programming/Writing Instructions in assembly, Here we don't have to care about the device or the instruction set/Architecture of CPU.  
    All modern Programming Languages support Many Architectures and Devices.  
    So we can write our instructions/logic in a high-level language like in plain English with some language-specific syntax.  
    ![High level language example](./../../img/JavaCodeHelloWorld.png)  

    And the Language converts them to Medium-level languages/Assembly languages/Machine code and **Executes** our logic.  
    This makes Creating software and applications fast and easy, all modern applications and technology are built using one or more high-level programming languages.  

    The logic we write is called **SOURCE CODE**, human-readable and easy to modify, this is then converted to respective device-specific instructions by the language in one of two ways(Compilation or Interpretation).  

    FORTRAN(Formula Translation) was a good example of a high-level language, the code is 20x times shorter than machine/assembly code.  
    But FORTRAN is device-specific, i.e, needed to change codebase (or) at-least recompile it for each device.  

    COBOL(Common Business Oriented Language) was invented to address platform independence.  
    A compiler for each machine is created first, then COBOL source code is given to that *COBOL compiler* to execute.  
    So despite the architecture, the code will be the same for all devices.  

    | year | language |
    | ---- | -------- |
    | 1957 | FORTRAN  |
    | 1958 | ALGOL    |
    | 1959 | COBOL    |
    | 1970 | Pascal   |

---

### Compilation vs Interpretation  

Each Programming Language is different from others in  

- **Syntax**
  - rules followed by it.
  - principles the languages uses.
  - features it provides.
  - the order of execution.
- **Uses** : Language can be majorly used for
  - Web Development
  - Mobile Applications
  - Server Applications
  - IOT Applications
  - Integrated Circuit Applications
  - Artificial Intelligence

The programming languages we are talking about are high-level programming languages,i.e these languages are easily understandable by user/programmer.  

Doesn't matter which Programming Language we use,(hereafter whenever we say programming language it is a high-level programming language like C, C++, Java, Javascript, Python, etc.,) it should be converted to machine code for the actual execution of our logic.  

We can convert the source code to machine code in one of two ways, Either by **COMPILATION** or **INTERPRETATION**.  

---

#### Compilation  

Programming Languages that support **COMPILATION** are called Compiled Languages.  

Compiled languages take user source code(written in English like syntax), then analyze it and compile it to assembly or machine-level code that the machine can understand.  

Advantages:  

- The compilation process is done only once but may take from minutes to hours.  
- Once done the output can be run very fast since instructions(machine code) are directly fed to the CPU.  

Disadvantages:  

- For different architectures, Operating systems, CPUs's the source code has to be compiled again.  
- Platform dependence, having to compile for each new platform independently is a slow and tedious process.  
- Code has to be compiled for small changes, for large projects this may take from minutes to hours.  
- Can't compile once and use it on any device.  
Ex: C language creates .out file in linux,.exe file in windows, can't interchange these files and execute.  

> (Note: there are compiled languages before C, but C implemented it really well and became industry standard, still being used 50 years after its invention.)  

Some Compiled Languages are  

| year | language                        |
| ---- | ------------------------------- |
| 1972 | [C](./../Languages/C.md)                |
| 1972 | SmallTalk                       |
| 1980 | [C++](./../Languages/C++.md)          |
| 1984 | MATLAB                          |
| 1986 | Objective-C                     |
| 1995 | [Java](./../Languages/Java.md)       |
| 1995 | Ruby                            |
| 2001 | [C#](./../Languages/Csharp.md)     |
| 2009 | Go                              |
| 2011 | [Kotlin](./../Languages/Kotlin.md) |
| 2014 | Swift                           |

![Compiled language](./../../img/Compiler.png)

---

#### Interpretation  

Programming Languages that support **INTERPRETATION** are called Interpreted Languages.  
Interpreted Languages take the source code line by line and feed it to the CPU for execution.  

Advantages:  

- No need for compilation for different devices, we just copy the source file to the device and execute it.  

Disadvantages:  

- Execution time is much longer compared to Compiled Languages.  
- what time we gain from skipping compilation we lose it while execution.  

Python is the most used Modern Interpreted Language.  

| year | language                                    |
| ---- | ------------------------------------------- |
| 1987 | Perl                                        |
| 1990 | [Python](./../Languages/Python.md)             |
| 1993 | Lua                                         |
| 1993 | R                                           |
| 1995 | [JavaScript](./../Languages/JavaScript.md) |
| 1995 | PHP                                         |

![Interpreter Language Execution](./../../img/Interpreter.svg)

**Speed Comparison**  
The below table shows the execution time in milliseconds, the lower the time the better performance.  
The same logic is run in different popular languages, code is precompiled.

| Language   | Execution time |
| ---------- | -------------- |
| C          | 6              |
| C++        | 7              |
| Java       | 15             |
| JavaScript | 900            |
| Python     | 1100           |

Depending on these results we choose our language of choice for developing an application.  

---
---

## Programming Paradigms  

Programming Languages are classified into Either Compiled or Interpreted.  

There is another Categorization Called Programming Paradigms that are used to Design the Language itself.  

These Paradigms are designed to make our code better scalable and maintainable.  

The Style/**Structure** given to **programming** logic irrespective of language is called **Programming Paradigm.**  

Major Use of Programming Paradigm is to Write

- Maintainable
- Scalable
- Easy to understand
- Easy to debug
- Non-Spaghetti code  

Each Programming Language Follows at At-least one paradigm some advanced languages follow two or more paradigms like Python or java.  
![Paradigms](./../../img/Paradigms.png)  

Here are some Programming Languages and Paradigms they support  

| Languages  | Imperative Paradigm                            | Declarative Paradigm |
| ---------- | ---------------------------------------------- | -------------------- |
| C          | Procedural,Parallel Processing                 | x                    |
| C++        | Procedural,Object-Oriented,Parallel Processing | x                    |
| C#         | Procedural,Object-Oriented                     | Functional           |
| Python     | Procedural,Object-Oriented                     | Functional           |
| Java       | Procedural,Object-Oriented                     | Functional           |
| JavaScript | x                                              | Functional           |

---  

Programming Paradigms are of two types

1. Imperative Paradigm
2. Declarative Paradigm

---

### Imperative Paradigm  

Imperative Paradigm is concerned with **How** the machine performs some logic.  
Ex: Providing directions to some address, Go straight take left on 5th street move 500m to right then go to 9th block room is 353.  

Here we *Explicitly* define the steps to be taken by our machine/CPU to perform.  

An Imperative programming language needs the user to implement the logic and be aware of the **Context**/control flow.  
The programmer has to manage the state of the control flow.  

Languages implementing Imperative Paradigm are often close to **How** a CPU works so will perform more efficiently.  
Ex: int a=10,b=20,c; c=(a+b); // here we are telling the program/language how to add two numbers.  

---

#### Procedural Paradigm  

The procedural Paradigm and Imperial paradigm are the same.  
>Procedural = Imperative  

In the Procedural Paradigm, we instruct the computer/CPU on how to do some task using basic statements(Conditional, Looping).  

This paradigm works in a top-down approach and treats data and procedures/methods as two different entities.  
Ex: C executes its code in a top-down approach, here we can't use a variable without declaring it first.  

Read [Procedural Paradigm](./ProceduralParadigm.md) document for more info.  

---

#### Object Oriented Paradigm  

Object-Oriented Paradigm works with objects.  
An Object is a combination of data and procedures/methods and is treated as a single unit.  
This is the most popular and widely used paradigm in 2020.  

Objects work by instantiating a **Class**, modularity and reusability are the main concerns of the OOP paradigm.  
Every Programming language that implements OOP provides  

1. Inheritance
2. Polymorphism
3. Abstraction
4. Encapsulation

Read [Object-Oriented Paradigm](./ObjectOrientedParadigm.md) document for more info.  

![Object Oriented Design](./../../img/OOPS.png)  

---

#### Parallel Processing Paradigm  

The parallel Processing paradigm works by dividing a given procedure or task into multiple parts and executing them simultaneously on multiple CPU cores.  

Many programming languages support parallel processing in multiple ways.  
C, C++ provides the best implementations of parallel paradigm.  

![Parallel Processing](./../../img/ParallelProcessing.png)  

---

### Declarative Paradigm  

The Declarative paradigm is concerned with **What** the developer/programmer wants to perform.  

We don't care how the program/logic/language works under the hood, just that it can perform a given task and return an appropriate result.  

Here the programmer defines what he want's to be done and the language takes care of execution.  

Ex: Instead of providing directions to our home, we give them our address and they get there however they can.  

Every(almost all) Declarative Paradigms have some imperative abstractions.  
i.e we can only tell **what to do** when the computer/language/logic **already knows how to do** it.  

Ex: `str. length()` is a method that returns how many characters are in a given string, we don't care/mind how this is actually implemented but just want accurate result when we ask it. `str. length('hello')=5`

Programmer declares what to do and expects a specific result.  
Ex: `select * from emp;` here we want our database to fetch details of emp table, we don't care how the database searches or how it stores the data.  

---

#### Logical Paradigm  

Logical Programming Paradigm is based on **Formal Logic/Mathematical Logic**.  

We use logical programming when  

- the relations between **facts and rules**, can help us solve a problem.  
- the workloads benefit from dynamic thinking/logical thinking.  
- we have to express our programming logic(code) in pure mathematical form  
- it is not clear what type of functions should be used.  

In Logical Paradigm, we are not concerned with  

- actual logical implementation  
- which functions are used to achieve the result  

Ex: "T is true if E and F are true or X is false" is a logical statement, "T is true" is a fact.  

The logical paradigm varies depending on the context.  
To solve a problem using the logical paradigm, we need a knowledge base containing facts, rules, relations.  
The most used logical programming language is Prolog.  

Nowadays a lot of programmers are using logical paradigms to teach machines how to think logically(machine learning).  

We provide a knowledge base containing all the information needed.  
Then inference/logic is used to solve the problem by taking the data from the knowledge base and finding the best possible solution(machine learning and deep learning).  

The logical Paradigm is not invented for machine learning but is being heavily used in that field nowadays.  

---

#### Functional Paradigm  

The functional Paradigm is the most used Declarative Paradigm.  
Here We define **What** to do, rather than defining **how** to do it.  
This is based and works similar to Mathematical functions.  
That is we can perform logics on abstract concepts rather than on implementation details, we can chain outputs to get new results, just like in maths.  
**Here is an example image of how functions in math works**  
![Math Functions](./../../img/MathFunction.png)  

Advantages:  

- In the Functional Paradigm we write our logic by applying and composing functions.  
- We don't deal with imperative logic(how the implementation is achieved).  
- Can chain the output of one function to another function's input.  
- Pure Functional Language Doesn't support loops, conditions that try to implement logic.  
- Results in a bug-free and efficient codebase.  
- Supports nested functions.  

The only major drawback is these languages require large memory space to execute.  

Most modern programming languages are Functional Programming Languages.  
Ex: Python, Javascript, Java.  

Refer [Functional Programming Paradigm Document](./FunctionalParadigm.md) for more details.  

![Functional Programming](./../../img/FunctionalProgramming.png)  

---  

#### Database Paradigm  

Database Paradigm can be considered the best example of Declarative Paradigm.  

We are only giving/using existing instructions and not creating any logic.  

Database Paradigm is concerned with data and its movement.  

Statements are defined based on data(changes depending on the type/size of data present) rather than hard coding the steps of execution.  

Imperative Programming languages are used to develop abstraction for the database paradigm.  

Out of many languages developed for database applications, SQL stuck around and is the dominating one(most used) in the Enterprise space.  

SQL is used to filter, transform, aggregate(combine small things to create big things) data from a database.  
>Ex: select * from emp where sal>1500;  

Here the database engine will perform logic for

- going inside the table
- filtering the data with given condition
- displaying in on the console  

Refer [Database Paradigm](./DataBaseParadigm.md) document for more details.  

### Useful Documents

- [Procedural Paradigm](./ProceduralParadigm.md)
- [Object-Oriented Paradigm](./ObjectOrientedParadigm.md)
- [Functional Paradigm](./FunctionalParadigm.md)
- [Database Paradigm](./DataBaseParadigm.md)

- [C](./../Languages/C.md)
- [C++](./../Languages/C++.md)
- [Java](./../Languages/Java.md)
- [C#](./../Languages/Csharp.md)
- [Kotlin](./../Languages/Kotlin.md)
- [Python](./../Languages/Python.md)
- [JavaScript](./../Languages/JavaScript.md)

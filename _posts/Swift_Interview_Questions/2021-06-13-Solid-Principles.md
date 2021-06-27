---
title: "Solid Principles"
layout: post
category: Sw_Int_Qst
tag: Solid Principles
---

The main intention of this architecture is to make our codebase more

- Understandable
- Flexible
- Maintainable

This architecture was broadly Implemented by **Robert C Martin** , *Uncle bob*, author of Viper architecture.

Solid Is an Acronym created By Micheal feathers

## S O L I D Defenitions

The acronym of SOLID can be described as below

###  Single Responsibility Principle:

> A class should have one and only one reason to change, meaning that a class should have only one job.

One effective way of conforming to single responsibilty principle is to reduce the task to small number of steps and grouping the tasks into specific classes. This will make the code more or less self documenting.

Single responsibity will make error debugging more localised. The unit test coverage of the project can be widely increased by following this method

Protocol oriented development if used correctly would vastly help with single responsibility in swift

------

### Open Closed Principle

> Software entities *(classes, modules, functions etc)* should be open for extension, but closed for modification

The code should be easy to extend but the base logic should not be modifieable.

--> loginc ase, apart from validation, in new project we have to query the databse to check if the username is already taken.

--> Base class a with strict requirements `final`. Now new classes conforming to this class can add new stuff but the strict items cannot be modified

### Liskov Substitution Principle

> Objects in a program should be replaceable with instanes of their subtypes without altering the correctness of the program.

--> Protocol oriented programming is itself in its essense.

### Interface Segregation Principle

> Clients should not be forced to depend upon interfaces that they do not use

### Dependancy Inversion Principle

> High-Level modules should not depend upon low-level modules. Both should depend upon abstractions.
>
> Abstactions should not depend upon details. Detail should depend upon abstractions.
---
title: "Solid Principles"
layout: post
category: Solid Principles
tag: Solid Principles
---



<i>Lets all of us agree that, during some point in out career, we had a chance to `review` some code written by someone and, we had to ask ourselves, what have I done in all my previous lives to endure this hell. </i>

<i> The funny thing to also agree is the code that you reviewed, might have been written by yourselves. </i>

<i>Don't smirk like you haven't written any sphagetty code Mr. </i>

<i>These things happen, It's normal. We all were stupid at some point in our lives. Everyone writes sphagetty code. Trust me, I just wrote something a few minutes back. [I'm Kidding of course, Dont do that] </i>

<i>You wish somewhere someone gave a thought on how to **reduce all this hell** and, wished there were some guidelines on how **not to code** something, that would make the person who maintaines your code, not to gauge his eyeballs out. </i>

<i>And Guess what, here enters SOLID Principles.</i>

Solid Principles are basically guidelines on how to write efficient code, that can be maintainable and flexible in the future Iterations.

Coding with keeping SOLID Principles in our mind will also make our code more

- Understandable
- Flexible
- Maintainable
- Testable

<i>Yeah, who writes test cases anyway..??  If you thought so, you are in soo much of trouble dude. You better write those test cases as your next appraisal depends on it.</i>

*This architecture was broadly Implemented by **Robert C Martin** , Uncle bob, author of Viper architecture.*

<i>Lets Code our new side project in viper architecture, SAID NO ONE EVER </i>

<i>Sample Cooode</i>

------





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
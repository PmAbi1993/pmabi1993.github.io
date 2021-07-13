---
title: "Single Responsibility Principle"
layout: post
category: Solid Principles
tag: Single Responsibility
---

While trying to conform to solid prininciples, Single responsibility principle is by far something that would help you the most.

Single Responsibility Principle or SRP says

> A class should have one and only one reason to change, meaning that a class should have only one job.
>

<i> That means don't stuff everything in a class and regeret later. Stuffing code in a class is for noobs. You may feel cool at present, but I will be there with a `I TOLD YOU SOOO`, when you will pull out your hair trying to debug the poorly written un documented code that has been sitting for releases...</i>

Single responsibility can be achieved if we start to think every task as a subset of tasks. 

A class should have a main responsibility and multiple sub responsibilities each constrained to its own classes. 

Moving every code you have written in view controller to a class called viewModel or Presenter is not desireable either. Now you will have to face  fat View model or fat presenter in place of fat view controllers. A poorly built fat class can hinder your testing and reduce debugging efficiency in the long run.

<i> I know why you are happy!! These cases are only applicable to people who write test cases and debug the code, right?. Let that one merge from the new guy mess up the core. I will be here again to watch your world burn 😈 </i>

## BreakDown to Subresponsibilities

Lets assume an example to achieving SRP in a situation we use in our daily tasks

### Task

Fetch a user information from the api, cache the images and store the data inside core data for offline functonality.

If we create a class called `UserData` and handle all the functions above listed inside the class, we might end up with a humongous class that in a way get harder to test and debug once an error occurs.

We also have to note that, once the class becomes too big and too cluttered, subclassing this class would result in availability of some redundant tasks and method in the superclass which the subclasses should have no need of.

### Solution

The solution to this is to break down tasks into multiple submodules.

We can breadkown the above task into:

1.  Fetch the userdata from internet
2.  Decode the data and create suffiecient models
3.  Download and Cahe the necessary inforamtion
4.  Save necessary items into the database.

Create seperate modules or classes for the above mentioned tasks and we can easily group the tasks to relatable modules.
Most of these tasks can be done more efficiently if we can compartmentalise them, use generics to handle relatable data etc.

So some modules for tasks can be further reduced and efficiency can be increased further. 

This in turn increases the testability and code quality.


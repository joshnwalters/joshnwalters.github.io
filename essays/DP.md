---
layout: essay
type: essay
title: Design Patterns
# All dates must be YYYY-MM-DD format!
date: 2019-04-27
labels:
  - Software Engineering
  - Design Patterns
---

Whether you're writing simple programs or massive libraries of code, things can quickly get out of hand without proper forethought and desing. Luckily for all aspiring software engineers, including myself, some smart people have already learned the hard lessons of software design patterns and made it available for us.

The most useful design pattern in my opinion would have to be the factory design pattern. The factory design pattern is an object-oriented design pattern that allows a user to create and access subclasses without needing to know any knowledge of the underlying logic. The classic examples include a superclass of car, or animals. For the sake of originality, I will use the example climate. Climate is a super class that includes several subclasses, including tropical, tundra, temperate, etc. From the superclass climate, we may do things like create a new instance of a tropical climate and set and get variables like temperature, rainfall, the list goes on. This can all be done at runtime, without needing to know what climate a user would need.

The next design pattern I will descuss is the adapter design pattern. If you have ever travelled to another continent, you may have ran into the problem where you go to charge your cell phone, but the socket in the wall is some crazy contraption with two small holes in it, vice the classic two- or three-pronged plug we're used to here in the States. An adapter is a life saver in those situations, just as the adapter design pattern allows you to join two otherwise uncompatible interfaces.

The final design pattern I will discuss is the strategy design pattern. In this pattern, we change class behaviors at runtime, based upon the behavior of a "context object". For example, let's say we have a program where a user can enter a message into our program, and also a function, encrypt or decrypt. The user simply submits the message, and whether he would like to run our encrytpion or decryption algorithm. Both of these pieces of information are passed into the context object, and the given method is ran on the data.

These were just three of many design patterns out there, there are several books and websites where you can learn more. The material is outrageously practical for quality software design. Next time you sit down to solve a new software problem, definitely review the different design patterns that may make your project more practical.

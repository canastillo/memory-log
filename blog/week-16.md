---
cover: >-
  https://images.unsplash.com/photo-1611338631743-b0362363f417?crop=entropy&cs=tinysrgb&fm=jpg&ixid=MnwxOTcwMjR8MHwxfHNlYXJjaHw1fHx3cmVzdGxpbmd8ZW58MHx8fHwxNjU4ODc2MjQ2&ixlib=rb-1.2.1&q=80
coverY: 15.037974683544304
---

# Interviewmania!

During this week, we had the first round of the interviewmania. This time, it was my turn to be the interviewer, and while preparing the interview, I had the chance to refresh or learn some new topics:

### OOP

The four pillars of OOP:

**Encapsulation** -> Each object takes charge of its own state, and the only way for the other elements of the system to interact with it, is through the methods of the objects (the getters and setters).

**Abstraction** -> From the outside, the objects are like black boxes: they don't know how methods are implemented, and they don't need to. They only have to know how to interact with the object (its methods).

**Inheritance**-> Inheritance allows you to establish like a hierarchy of classes. It allows to reuse common methods and attributes between classes, without needing to write it multiple times.

P**olymorphism** -> The way I understand this, is to have a different behavior despite using the same method (through override, which happens at runtime, and overload, which happens at compile time).

### SOLID

This is a series of principles that guide the way to design the systems.It has multiple objectives, but overall, it aims to make the code maintainable, so it is easier to modify it in order to fix bugs, make refactors or add functionalities. In other words: low coupling and high cohesion.\


**Single Responsibility**

Each class should take care of only one thing within the system. Since they only do one thing, it's easier to make sure they do it good.



**Open/Closed**

The parts of the system have to be open to add new functionalities, but closed for modifying them, that is, when something new needs to be added, new code must be written, instead of modifying the existing one.

The objective here is not to change code that is already working every time that the requirements change. Here are used tools like inheritance and polymorphism.&#x20;



**Liskov Substitution**

The system should be able to interact with the subclasses of a superclass as if they were the superclass itself. No element of the system should behave different when interacting with any of the descendants of a class.



**Interface Segregation**

Sometimes, even though we respect the Single Responsibility principle, we may have a super big class which many other classes interact with, however, not all of these other classes should have access to all the methods of this super big class when they only need a small set of methods from it. A client should not be exposed to methods it doesn't need.

Interface segregation is about hiding parts of the class to the rest of classes. You cannot interact directly with the class, but through interfaces that tell you to which part of the class you have access.\


**Dependency Inversion**

Concrete implementations should not depend on concrete implementations, but of abstract layers. So, communications between the components of the system is always through interfaces.

### Casting vs Parsing

This is something I started investigating about. I'm yet not so sure on the differences, but as far as I understand, casting happens when trying to change from one data type to another one which is compatible (like int and float), while parsing is more about syntax and formatting, taking some characters and give them a "different meaning" (like parsing from string to int, or during compilation, the compiler uses parsing to interpret the instructions).



That's all for this week, bye!


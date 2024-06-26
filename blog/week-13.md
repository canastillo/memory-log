---
cover: >-
  https://images.unsplash.com/photo-1588239034647-25783cbfcfc1?crop=entropy&cs=tinysrgb&fm=jpg&ixid=MnwxOTcwMjR8MHwxfHNlYXJjaHwyfHxqYXZhfGVufDB8fHx8MTY1NzA3NzEyNQ&ixlib=rb-1.2.1&q=80
coverY: 784.8101265822785
---

# Open Source - Round 2

This week I focused on learning about Java. Here's a little of what I learned:

## Getting to know the enemy <a href="#java" id="java"></a>

Just kidding. Certainly I don't like Java, but I've always known that I feel that way because I haven't given myself the chance to actually learn it and understand it. The only experience I have had with it was during an awful subject at university. So yeah, I'm giving it a shot.

### A lot of Js

First things first. There's a lot of Java vocabulary that confuses me a lot, so I needed to understand what these words meant.&#x20;

* **JDK:** Java Development Kit. Tools for compiling the code.
* **JRE:** Java Runtime Environment. Tools for running the code.
* **JVM:** Java Virtual Machine.
* **JSE**: Java Standard Edition. Includes the JDK and JRE. It basically says what type of JDK and JRE is being used.

These concepts aren't quite different with each other. In fact, they are one inside the other. The JDK includes the JRE and the JRE includes the JVM.

![This graph is cool, isn't it?](<../.gitbook/assets/image (7).png>)

**Note:** Java has evolved for implementing a module system in which it isn't that necessary to have a JRE.

{% hint style="info" %}
Did you know Java has a mascot? It is called Duke. Nobody knows what the heck is it. Probably a demon from hell, just like Java.
{% endhint %}

### The JVM

Java is famous because of its "Write once, run anywhere" philosophy, but I hadn't understand what that meant, how is it achieved and why is so cool about it.

Well, it all happens thanks to the Java Virtual Machine. In other languages, like C or C++, you need to have your source code on your machine, and compile it to generate an executable that works only on that OS. So, the executable generated by the compiler on a Linux distro, wouldn't work on a PC, for example. Java solved this with the JVM.&#x20;

The java source code (.java) is also compiled, but the Java compiler (javac) instead of generating executables, generates Java bytecode (.class), which can't be interpreted by the machine itself, but by the JVM. So, as long as you have a JVM installed, your code will be run no matter the OS of the machine.

{% hint style="info" %}
Did you know that, before Java 9, the versions of Java were formatted as 1.x? So, Java versions go like: 1.6, 1.7, 1.8, 9, 10, 11, and so on. Why? 'Cause Java developers like to suffer and make everyone else suffer. Nah just kidding, it's because of marketing stuff.
{% endhint %}

### Memory management

This is how the stack and the heap work in Java.

* **Stack:** stores primitives and references.
* **Heap:** stores objects.

So, when we do `int a = 10;` it is stored in the stack. In the other hand, when we do `Card card1 = new Card();` the new object is stored in the heap, and the card variable stores in the stack a reference to that object. When we go `card2 = card1`, we don't create a new object, that is, we are not copying it, we're just storing another reference in the stack that points to the same object in the heap.

#### The stack

![](<../.gitbook/assets/image (12).png>)

In the stack, the variables don't just pile up one after another. There are like sections or blocks, one per function call. If this stacks gets filled up, we get the so called StackOverflow error.

#### The heap

The heap is divided into three sections.

* **Young generation**: Where the new created objects fall into.
* **Old generation**: Objects with some time alive are moved into here.
* **Permanent generation:** Java reserves this section for all the meta data used by the JVM.

When the heap is full, we get the OutOfMemory error. Java cleans this sections with the garbage collector, which I'm probably search about during this week.

## Open Source

So, I searched for Java projects to contribute. I picked these:

* [Micronaut](https://github.com/micronaut-projects/micronaut-core)
* [Hibernate](https://github.com/hibernate/hibernate-orm)
* [OpenRefine](https://github.com/OpenRefine/OpenRefine/issues/5004)

On May 30th (Thursday), I left a comment for this Micronaut issue: [https://github.com/micronaut-projects/micronaut-core/issues/7275](https://github.com/micronaut-projects/micronaut-core/issues/7275)

On July 1st (Friday) I asked for this Hibernate issue: [https://hibernate.atlassian.net/browse/HHH-15378](https://hibernate.atlassian.net/browse/HHH-15378); and this OpenRefine issue: [https://github.com/OpenRefine/OpenRefine/issues/5004](https://github.com/OpenRefine/OpenRefine/issues/5004)

At first, I was thinking on waiting for the maintainers' approval but, since there's only one week left, I decided to not to wait and start working immediately. Anyway, I hadn't had the chance to start working on any issue, until today (Tuesday), mainly 'cause I spent a lot of time working on the EPC docs, but I only managed to set up the environment for the Micronaut project, so yeah, I haven't written not even a line of code.

I started with the Micronaut issue because someone gave me the green light on Sunday.

Actually, I'm not even sure if the environment is ready, 'cause I get some errors from the console. I tried getting some help in the gitter chats for Micronaut:

{% embed url="https://gitter.im/micronautfw/questions" %}

{% embed url="https://gitter.im/micronautfw/espanol" %}

However, I hope I can solve it tomorrow. After it, I may take another issue without the "good first issue" label or I may go for the OpenRefine issue. In that issue I didn't receive an approval, but people started discussing about the problem and removed the "good first issue" tag, and I gotta search for harder issues.




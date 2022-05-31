---
cover: >-
  https://images.unsplash.com/photo-1569017388730-020b5f80a004?crop=entropy&cs=tinysrgb&fm=jpg&ixid=MnwxOTcwMjR8MHwxfHNlYXJjaHw1fHxvcGVuJTIwc291cmNlfGVufDB8fHx8MTY1MzM1ODYzMQ&ixlib=rb-1.2.1&q=80
coverY: 460.2937720329025
---

# Open Source - Round 1

It’s been a long time since the last time I wrote in this blog. A lot of things have happened. Anyways, I’ll focus on the learnings of the last week.

## Are you an expert? <a href="#coding_horror" id="coding_horror"></a>

A friend in the apprenticeship program shared with me a couple of neat articles on failure and being an expert. They are written by Jeff Atwood, the creator of Stack Overflow. &#x20;

First, in the post about being an expert, Jeff says this definition of an expert:&#x20;

> "Being an expert isn't telling other people what you know. It's understanding **what questions to ask**, and flexibly applying your knowledge to the **specific situation** at hand".

This reminds me of the course Learning How to Learn, where Barbar Oakley said that expertise doesn’t come just from chunking and nothing more, but manifests when we learn to **discern when to use each chunk**. I liked a lot the last phrase of the post:&#x20;

> "Don't be the guy telling everyone what to do. **Be the guy asking all the questions"**.&#x20;

Then, in the article about failure, Jeff mentions this fact about Alva Edison, who failed a thousand times before finding the right way to make the light bulb, but never thought that he had been wasting time, ‘cause he had found a thousand ways that didn’t work, each time **getting closer and closer** to the final answer.&#x20;

This is the way that success is reached: through failure. That’s why Charles Bosk, a sociologist, after interviewing doctors that had been fired from training programs, jumped to the conclusion that the doctors that **were going to be good surgeons** were those **admitting to make mistakes** all the time:&#x20;

> “They were the best. They had the ability to **rethink everything** that they'd done and **imagine how they might have done it differently**.”&#x20;

So, yeah, our virtue isn’t just in failing, but on reflecting on it and figuring out what we should do different next time.&#x20;

This is Jeff Atwood's blog, in case you are interested:

{% embed url="https://blog.codinghorror.com/" %}

## `make essay` <a href="#gnu_make" id="gnu_make"></a>

Since we are in a phase where **we have to get into the Open Source **_****_** community**, we were assigned some questions we have to answer by reading code on Github. I chose one about **how dbms manage indexes**. So, after exploring Mysql and Postgres repos, I found in both of them something called _make_.&#x20;

Then I remembered I had seen something similar when working with ledger. Actually, ledger uses _cmake_, but the idea is the same. They are both **build automation tools**. In other words, software that allows you to write instructions (called _rules_), that help you when **compiling a complex project**.&#x20;

![It is a GNU library](<../.gitbook/assets/image (3) (1).png>)

In fact, I even heard someone saying you can use make for other things that have nothing to do with programming, but as I mentioned earlier, it is intended to automate the build process. That is, **get a binary from source code files.**&#x20;

It works with _makefiles:_ we simply gotta write the commands we want to add and the instructions that must occur when that command is invoked. Here we got an example:

![](<../.gitbook/assets/image (8) (1).png>)

The file must be named `Makefile`.&#x20;

Following this example above, if we write on the command line `make build`, the instructions below line 7 will be executed. If we write `make clean`, instructions below line 4 will be executed. If we write `make all` (or just `make`, ‘cause that would execute the first command), command `clean` would be executed and then command `build` would be executed.

It's that easy!

{% hint style="info" %}
Note: **Indentation** in a Makefile is important!
{% endhint %}

## Testing

I have been learning about testing with one of my mentors. Here are which I consider the most important points:

* The first tests are the unit test, which check a **single responsibility.**
* **Mocks** are usually used in **unit testing.**
* Usually tests are divided into **given** (the initial conditions), **when** (the functionality we want to test) and **then** (the expected result).
* We use the keyword **assert** when testing the **output** and **verify** when testing the **behaviour.**
* When it comes to UI, testing occurs on **components** (we test the **state**).

## On open source <a href="#open_source" id="open_source"></a>

This week I have been exploring a lot of repos, trying to find an issue which I can tackle. I haven't found a project where I feel comfortable giving it a shot. Probably I'm gonna start with something little until I feel confident with trying something bigger. The deadline is in one week and have no time to waste.

However, I have noticed how important proper documentation is. As a project grows and grows, it may become critical to have comments describing functions, files, and the infrastructure of the code.

Also, each project has its own rules on how to contribute: with forks, cloning mirrors, using PRs, assigning issues or taking the first good answer, etc. It's important to read the guidelines and have a good communication.

I think that's all for this week. See ya!

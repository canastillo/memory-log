---
cover: >-
  https://images.unsplash.com/photo-1488590528505-98d2b5aba04b?crop=entropy&cs=tinysrgb&fm=jpg&ixid=MnwxOTcwMjR8MHwxfHNlYXJjaHwxMHx8amF2YXxlbnwwfHx8fDE2NTc1NzUwNzA&ixlib=rb-1.2.1&q=80
coverY: 0
---

# Circuit breaker

For this phase, I tried picking issues that were easy enough to help me get to know the project, and then go picking harder and harder issues as I was finishing them, but in repos that would take me out of my comfort zone, that is, no Javascript or Python projects, and no issues that were somehow frontend or UI related.

Although I picked "good first issues", I'm still dealing with the first of three issues. Here I share with you my learnings and insights, and what would I do different.

## My contribution

So, I picked an issue from the Micronaut framework repository. This is a framework that helps you develop Java microservices. This particular problem is related to the CircuitBreaker, the Micronaut's implementation of the design pattern of the same name.

The problem was that the CircuitBreaker would throw the original error when the circuit is open, instead of telling the user that there was an error because of the circuit being open. In order to not to change the original behaviour, the suggestion was to add an option for the user to specify in the annotation which exceptions should not be rethrown.

You can see the issue and the discussion here:

{% embed url="https://github.com/micronaut-projects/micronaut-core/issues/7275" %}

And here you can see the changes I've made so far:

{% embed url="https://github.com/canastillo/micronaut-core/commits/exclude-exception-rethrown" %}

## The good part

### Things I learned

* How Java works (I talked a little about that last week).
* To easily switch between Java versions with jEnv (and [this article](https://chamikakasun.medium.com/how-to-manage-multiple-java-version-in-macos-e5421345f6d0)).
* To work with IntelliJ IDEA, Gradle and the build.gradle file (for building and running both from the UI and the terminal. Also did some debugging).
* About the Microservices architectural pattern.
* About the Circuit Breaker pattern, which is based on the Retry pattern, and the importance of resilience.
* About Java dependencies, Maven repositories and "publishing to local".
* About creating REST APIs with Micronaut.

### Things I think I did good

* Didn't wait for someone's approval to start working on an issue, I just made sure it was an active repo.
* Not expecting to fully understand the whole codebase to start coding.
* Ask for help trough different channels (in the issue thread, on the official Gitter server of the project, and on the Encora slack).

Here are some screenshots of my conversations (you can read the issue thread from the [link above](week-14.md#my-contribution)):

![On https://gitter.im/micronautfw/questions](<../.gitbook/assets/image (11).png>)

![On https://gitter.im/micronautfw/espanol](<../.gitbook/assets/image (2) (1).png>)

As you can see, the README for contributing was outdated. This was a problem at the beginning, when I barely had an idea of what was going on and nothing made any sense but, I managed to have my environment ready anyway.

![](<../.gitbook/assets/image (14).png>)

![](<../.gitbook/assets/image (15) (1).png>)

I used the java slack channel for more specific and technical questions.

## What went wrong

I think there were mainly three mistakes.

First, I didn't organize myself properly and let activities of the previous phase impact on my activities for this phase. Because of that, I lost pretty much one week (I didn't actually start until last Tuesday).

The second one is, I underestimated the issue because of the "good first issue" label. It is certainly a short issue, but I didn't consider the uncertainty factor: I hadn't truly dealt with Java before this, so it was a completely different environment for me. Also, I picked quite a big project with a considerably big codebase, in which is easy to get lost when you are not sure of what you are looking for.

The last thing is, I felt pressured because I had only one week left, so I tried like, to skip steps. I thought the problem was as straight forward as adding a conditional. I mean, it isn't that hard, but I wanted to tackle the problem without even knowing what a Circuit Breaker was and without having used Micronaut not even once in my life. There was a point where I realized I had to make an app with Micronaut if I wanted to see my changes in action (yep, I didn't think of it until three days later), so I spent hours searching for "simple" examples and trying to get them running. At the end I didn't make it. Next day it took me 2 hours get up and running my own app.

I focused too much on having a task ready, mark it as done in the to-dos list, instead of reading and searching until I fully understood what was the problem and the possible solutions.

## What I'd do different

* Don't let previous tasks slow me down. It may require extra time, but it's important not to focus on one thing only (for many days in a row I mean). Be more multitasking.
* Consider the uncertainty.
* Make sure I fully understand the requirements before starting to write code.
* I made questions and asked for help, but it would have been better to reach out sooner.
* Having clear in the mind what the problem is and the possible alternatives is necessary for making good questions.

## What's next?

I'm going to keep working on this issue (testing the code mainly) and solve at least other two, while trying not to leave aside the activities of this coming phase.

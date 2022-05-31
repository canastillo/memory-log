---
cover: >-
  https://images.unsplash.com/photo-1555066931-4365d14bab8c?crop=entropy&cs=tinysrgb&fm=jpg&ixid=MnwxOTcwMjR8MHwxfHNlYXJjaHw2fHxjb2Rpbmd8ZW58MHx8fHwxNjUzODE3NzI5&ixlib=rb-1.2.1&q=80
coverY: 0
---

# Learning to read code

This first round of the Open Source phase is over, and I couldn't feel happier. Now that I read it out loud it sounds bad. I'm not happy that it's over. I'm happy with my results. I would love to have a better answer for my question though.&#x20;

The point is, I gave my best effort and enjoyed a lot the process. At the beginning I was very doubtful of myself but everything turned out good. I'm going into the next phase with a lot of learnings and a very good experience. Here's what I learned.

![](<../.gitbook/assets/image (11).png>)

## About contributing on Open Source

I learned there's a lot different Open Source communities. The process for contributing may vary in each project 'cause each community supporting it is different: The way the communication happens, the way of asking for or assigning issues, the rules for creating issues or PRs, how branches are used, how versioning works, and code style. There are huge projects with a lot of documentation and others that don't even have a specific guideline or standard for writing PRs.

You cannot just go and ask for an issue. I mean yeah, but there are things to consider before: When the last commit was, how many and how often issues and PRs are closed, how big the project and the community is, how friendly they are, how actively do they participate and comment.

Overall, by making my contribution I learned how to create the PR, comparing a branch in the base repo with a branch in my fork, and learned that people can review your code and make suggestions, which you can commit one by one or all together in a batch.

![](<../.gitbook/assets/image (7).png>)

I also learned how to better use the tools that Github brings for discovering and exploring repositories. I'm super happy 'cause I discovered projects which I'm pretty interesting in and want to make contributions to. Now I can tour with confidence through the threads in the repos 'cause now I have a better understanding on what is going on.

## About DBMS

In the process of answering my question, I learned a lot about the logic behind a relational database and a little about C syntax.

Some of those concepts were:

* **System catalog:** It's basically a set of tables which describe the database, as well as the system settings. That is, it documents the database objects: things like tables, indexes, views and stored procedures. I couldn't find any determining fact on this but, as far as I understood, this is for relational DBMS only. Since there are no relations in NoSQL databases, I guess the collections describe themselves?
* **Partitioning:** It's about splitting up a table into smaller tables, so that the queries don't need to access all of the data, so they are less expensive (the bring less data) and more efficient (there are less records to scan). This partitioning may be vertical (split by columns, keeping the same amount of rows) or horizontal (split by rows, keeping same amount of columns).
* **ACID:** Stands for Atomicity, Consistency, Isolation, and Durability. These are properties that the relational databases transactions must meet in order for the database system to be considered reliable. **Atomicity** means that each transaction is considered to be an indivisible series of operations. If a single operation fails, all operations are cancelled. **Consistency** means that the rules and constraints of the database are followed at all times. **Isolation** means that data is only visible in the database once the transaction has ended. **Durability** means that the data is saved to a permanent storage once a transaction is saved.
* **Locks**: These are used to ensure the integrity of data. Processes lock the database resource while using so that no other process is permitted to change the locked data. Locking facilitates the ACID properties of the transactions.
* **Deadlock**: This happens when two or more transactions are waiting indefinitely for one another to give up locks.

![](<../.gitbook/assets/image (12).png>)

That's all for this week. Bye!

---
cover: >-
  https://images.unsplash.com/photo-1616990277552-3db5bca0ce13?crop=entropy&cs=tinysrgb&fm=jpg&ixid=MnwxOTcwMjR8MHwxfHNlYXJjaHw4fHxtaXN0YWtlc3xlbnwwfHx8fDE2NTkzOTQ1Mzg&ixlib=rb-1.2.1&q=80
coverY: -165.2299578059072
---

# You are not your backhand

This week we were assigned only three lectures, but I found it really pleasant that they all felt connected to each other.

Overall, the common topic was "the power of the mind". Well, kinda. The thing is, it is hard to learn when we want to have everything under control. See it this way: if we control absolutely everything, that means we already know everything, and if we already know everythig, what is left to learn? Nothing!

Leaving room for mistakes leaves room for growth, and this is not possible if we judge ourselves based on our successes or mistakes.

The facts are the facts, no matter the opinions or biases. There's performance and goals, how far or close we are from our objectives don't define us as persons, **we are not our backhands**.

So, this "power of the mind" thing is about quiet all those inner voices that distract us from our goal. I takes a lot of practice and effort, but it's possible. Breathing exercises are cool for achieving this.

The "power" is in focusing and letting go.

Sounds kinda contradictory, but focusing on what you want to do, lets that "unconscious" part that knows how to do things, do them. When all the judgements cease, we truly concentrate on our goal, we let go 'cause we're not afraid of making mistakes, and with a loose body, we are able to reach the peak of our performance.

A cool trick for paying attention is to stop assuming we already know everything about a topic, having in mind that we can always learn something new.

### Technical stuff

This week I learned a little about docker and how it is different from virtual machines: while containers run directly within the host’s machine kernel, virtual machines are isolated from the rest of the system.

![](../.gitbook/assets/image.png)

> Virtual machines have host OS and the guest OS inside each VM. Guest OS can be any OS, like Linux or Windows, irrespective of host OS. In contrast, Docker containers host on a single physical server with a host OS, which shares among them. Sharing the host OS between containers makes them light and increases the boot time.
>
> \-Taken from [_Docker vs. Virtual Machines: Differences You Should Know_](https://cloudacademy.com/blog/docker-vs-virtual-machines-differences-you-should-know/)__

Also, I learned more about how CPUs work.&#x20;

Instructions are brought to the CPU from the RAM. Inside the CPU is the Control Unit, which receives the instructions stored in the RAM and decides which commands should be sent to which components. The ALU, which stands for Arithmetical Logic Unit, is the one who makes all the mathematical operations. This ALU may give an output, which is the actual result of the operation, or may give some flags, which say if certain condition has been met or not. These results are given back to the Control Unit and then stored back to the RAM.

![Illustrative example of how computers work](<../.gitbook/assets/image (1).png>)

The communication between these components happen through buses, which are wires. The address bus indicates which address in the memory is being accessed, the data bus is used to transfer the data, and the control bus is the one which indicates if data must be transmitted or received to be stored. This control bus often consists of two wires which are the set wire and the enable wire. Depending on which one is turned, is the action performed to the data at a given address. Some components may only have a set wire or none depending on whether it's a bus for communication two components only or it is shared between multiple components, or if communication is bidirectional.

Temporary data is stored in the registers. Registers are like RAM, but RAM stores instructions, numbers, letters and addresses, while registers store one number only, and they are for a specific data. That is, there's a register for instructions, there's a register for the inputs and output of the ALU, there's a register for the flags, and so on.



That's all for this week, bye!


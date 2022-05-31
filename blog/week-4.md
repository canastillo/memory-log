---
cover: >-
  https://images.unsplash.com/photo-1506702315536-dd8b83e2dcf9?crop=entropy&cs=srgb&fm=jpg&ixid=MnwxOTcwMjR8MHwxfHNlYXJjaHw1fHxtaXN0YWtlfGVufDB8fHx8MTY1MTUzMzY2Ng&ixlib=rb-1.2.1&q=85
coverY: -130.7052280311457
layout: editorial
---

# Fail fast, die hard

This week was a loooot about testing (the academic topics actually were a little harder for me than the ones in other weeks), but it was also about making mistakes, the importance of feedback and being human. _It doesn't have to be perfect_ we learned the previous week, and it's still true. We just gotta keep trying.

### How big tech companies search for failures <a href="#netflix_google_testing" id="netflix_google_testing"></a>

This week I was pretty interested in how Netflix would use its _Simian Army_ for **testing in production** (I mean what?).&#x20;

![](<../.gitbook/assets/image (7) (1).png>)

They had to do it this way because, the system is so big that simulating the whole environment would consume a lot of resources, and yet it wouldn't truly represent the real state of the project (it's literally impossible).

As far as I know, they don't use the army anymore, but it certainly is an interesting concept.

Meanwhile at Google, all the different projects are commited into one single branch (well, there are two actually), so they have tools for making sure everything works before submitting changes.

![](<../.gitbook/assets/image (4).png>)

From these talks a learned that **engineers usually don't like to make tests** (they claim that it's a waste of time) and that **tests consume computing resources**.&#x20;

I mean, it may seem obvious but I hadn't thought of it. Things like _sharding_, where a test gets to be divided into as many separate parts as you want and **each one gets its own execution engine**, are not good, folks, 'cause you may get a tiny benefit of seconds but you **double the number of resources** that the system is using to run that test.

Not good.

### Pretotyping

However, when we talk about testing, we are talking about products that are already created and we want them to operate well under difficult conditions. We don't want them to fail in the most critical moment. The thing is, projects can (and **must**) **fail** even before they are launched.

![Pretotyping at IBM](<../.gitbook/assets/image (11) (1) (1).png>)

I had never heard of _pretotyping_ before. It's about simulating an experience in order to know if what we want to build is what we should be building. It's about **testing the idea before fully committing to make it real**. I see it as having clear where is the finish line before jumping to the water in a swimming competition.&#x20;

The value of this is that before being misguided by opinions, we get facts, we get data about what the users want. The point is getting **feedback** as soon as possible.

### Failure... is often more illuminating

There's nothing bad in failing. Actually, we are al "doomed" to fail, as Alberto Savoia expresses in his _Law of Failure._ So, it even isn't about failing or not, it's about _when_, and what are we going to do about it.

The sooner we get this, the better. There is, for example, the aviation industry. They implemented the black boxes into the planes in order to know how and why the accidents happened. They **wanted feedback**. They didn't **pretend like nothing happened**. No. They faced the facts and had the willingness for **changing what had to be changed**.

This mentality of not feeling shame but having the courage to admit our mistakes (and being open to **tell the other ones what they are doing wrong**) is what helps us to be better professionals, and better persons.

### Mistake is what makes us human

I don't know if I fully agree with that phrase. Although, we certainly have the capacity to fail, opposite from animals, who cannot make errors. If they do, they die.

For us humans it's not that drastic. We have the capability to learn, to change, to be kinder. For me, that's the most important thing. At least, that's the way I define success. **Did you make connections with the people around you? Did you leave something good in every person that walked throught your life? Did you help someone feel or be better?**

It makes me happy to think that people like Feynman, who made big contributions to various fields in science, is often remembered by the close people to him as a human, before a scientist.

![](<../.gitbook/assets/image (1).png>)

I feel that fascinating stuff like quantum mechanics and computation, which show that at microscopical scale may happen things that we don't understand, yet so simple, provoke amazing and complex stuff, like the universe itself; all these things, **make no sense if we forget who we are and that we are not alone**.

Funny how I'm now trying to talk about humanity and being all good pals when two paragraphs ago I just mentioned one of the scientists involved in the Manhattan Project (yet I should investigate more about this).

Anyway, the moral here is, there's nothing wrong with failure. We are going to fail, the sooner the better. I thinks that's what this is all about. We can even see it on the scientific method. You cannot even prove when you are right, 'cause the next time you could fail. Laws and theories are nothing but humans saying what is **likely or unlikely to happen**, but you cannot be completely sure at all, until you are wrong. Then is when **you can be sure you are wrong**.

That's how we make advances in technology and science.

That's the way we progress: by **failure**.


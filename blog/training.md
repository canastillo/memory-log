---
cover: https://www.feda.net/wp-content/uploads/2017/09/funcional-training.jpg
coverY: 97.04641350210971
---

# Training

We spent the last three weeks on trainings for React, Java, and Spring boot. Here's an abstract of what I've been learning.

### React

These are JS topics actually but I learned them in the course:

* This operator `...` is called in different ways depending on how it is used: `rest` when is is used to take multiple variables into a single object/array, and `spread` when used to pull out the elements of an object/array.
* How to get and set properties in the local storage.
* There's something called alias destructuring which allows you to give a different name to a destructured property:&#x20;

```javascript
const obj = { x: 1 };

// Grabs obj.x as { x }
const { x } = obj;

// Grabs obj.x as as { otherName }
const { x: otherName } = obj;
```

Now, these are about react:

* In former versions of React, it was mandatory to place `import React from 'react'` at the top of every file in a React project. I didn't new that it was actually necessary in those files which return some jsx code, and it was required in order to be transformed into JS syntax.
* There are these concepts of controlled and uncontrolled components. This is a way of calling components which internal state is managed or not by the developer.
* CSS modules are another way of implementing styles to React components.
* Refs help us manage some DOM elements directly.
* There are different workarounds for this JSX limitation of only allowing rendering one element.
* The limitation above is based on the fact that in JS, we can return one thing only in functions.
* Learned about reducers for managing the state.
* How Context API is helpful and how to use through useContext.

### Java

* Record classes in Java are available since Java 14, and are classes which are intended to never change after they are created for the first time. They are immutable, and constructors, `equals`, `hashCode`, and `toString` methods are created automatically.
* Final and static methods cannot be overridden.
* Since Java 16 we got sealed classes, which are classes that determine to which classes they can inherit to.
* With the use of `this()`, we can chain constructors.
* Classes which "don't inherit from other classes" actually inherit from the Object class (everything in Java inherits from it).
* It is important to override the `toString`, `equals` and `hashCode` of our custom classes that inherit directly from Object.
* We can import all the static methods from a static class doing something like `import static MyStaticClass.*`
* The classpath is set of paths where the java compiler and the JVM must find needed classes to compile or execute other classes.
* Dealing with exceptions through a try-catch block or modifying the signature of the function being executed.
* A little about the garbage collector and how it trashes objects which are not being referenced by any variable.
* Reading and writting files with the `FileReader` and `FileWritter` classes (`BufferedReader` and `BufferedWritter` are actually a better choice, but they both need either a FileReader or FileWritter).
* To use lambda syntax and a little about streams.
* To use enums, the BigDecimal type, and dealing with dates and time
* Checked and unchecked (runtime) exceptions.
* When dealing with strings, it is always recommended to use the equals method, 'cause when using the == operator, it compares memory locations.
* Java has a string and integer pools (instead of creating new instances, the new variables point to the same memory positions).
* I thought the elements in hashsets would change their order each time we try to access them, but this is not true. The thing is that their order is determined by their hashcode, not by the order they were added to the collection, so, the order may vary from the order they were added, but their hashcode will always be the same, so their order is the same.
* There are Java specifications which may expose annotations, but we have to do the implementations.
* Both DAO and Repository are patterns for managing data, but are not the same. DAO can't be implemented using a repository. However, a repository can use a DAO for accessing underlying storage.

### Spring

* Spring isn't the same as Spring Boot. Spring is a framework for building backend applications, but it was super hard to configure. Spring Boot is a framework to help making configurations way easier and friendly.&#x20;
* About Application Context and Spring Beans (which are different from Java Beans).
* About dependency injection and `@Autowiring` annotation (Spring cannot inject a dependency into a class unless both of then are within the application context).
* When we are using annotations like `@Controller` or `@Service` in our classes, we know that they are being managed by Spring because they include the `@Component` annotation. These components are added to the app context when a component scan runs. This happens when we run our application (only if our Main class is at the root level of the app, above all other classes, and has the `@SpringBootApplication` annotation, which has the `@ComponentScan` annotation).
* &#x20;We can use the `application.propperties` file to give some configuration to our dependencies and creating profiles for different environments.
* All POJOs in Spring MUST have a default constructor.
* By default, Spring comes with jUnit for testing.

### Other things

* Your IDE can help you generate code automatically. I learnt how to generate constructors, getters, setters, override methods and more with IntelliJ.
* There's a technique called currying which allows you to pass parameters to functions at different moments, but I didn't go any deeper on that.
* With the exclude pathspec, we can add all the current changes to a commit, except those which we indicate: `git add --all -- ':!path/to/file1.txt'`


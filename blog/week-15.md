---
cover: >-
  https://images.unsplash.com/photo-1515879218367-8466d910aaa4?crop=entropy&cs=tinysrgb&fm=jpg&ixid=MnwxOTcwMjR8MHwxfHNlYXJjaHw0fHxjb2RlJTIwY2hhbGxlbmdlfGVufDB8fHx8MTY1ODE5MzU4NQ&ixlib=rb-1.2.1&q=80
coverY: 0
---

# More Java

Hi! This week I focused mainly on doing coding challenges with Java so, here is all the technical stuff I learned.

### Iterate arrays

There are different ways to loop an array:

* First of all, the for loop of course:

```
// This one uses indexes
for (int i = 0; i < myArr.length; i++) {
    System.out.println(myArr[i]);
}
```

* Enhanced loop (uses an external iterator):

```
// This one uses the elements
for(int element : myArr){  
    System.out.println(element);  
}
```

* forEach loop (uses an inner iterator):

```
// Pretty much like the one above
myArr.forEach(element -> {
    System.out.println(element);
});
```

* streams!

```
myArr.stream().forEach(element -> System.out.println(element));
```



Also, I got a refresher on how to loop over circular arrays:

```
 for (int i = startIndex; i < myArr.length + startIndex; i++)
     System.out.println(a[(i % myArr.length)]);
```

### HashMaps

I learned some useful methods for hashmaps!

We can use the `map.put()` method for inserting a new element in the hashmap, we just gotta give it the key and the value. However, we can use this same method for updating an existing mapping. In combination with `map.getOrDefault()` , we can increment a value in one line:

```
map.put(key, map.getOrDefault(key, 0) + 1);
```

In this way, if the key exists, we can get the previous value of the key and update it. If it doesn't exist, it starts the counter with 1.

Anyway, my favorite one was the `map.compute()` method, which allows us to update the values of the map:

```
// Another way of incrementing the value or creating the entry!
map.compute(key, (k, v) -> (v == null) ? 1 : v + 1)
```

We also got the `putIfAbsent()` method, which inserts a new mapping only if it doesn't exist previously (so, it doesn't make any update).

### HashSets

In one of the HackerRank challenges, I needed a HashMap but without the values. Then I found out that what I needed was a HashSet.&#x20;

Since it is an implementation of a Set, there's no need to check for duplicates (when calling `hashset.add(element)`, it will return false and won't add any element if this element already exists).&#x20;

### Interfaces vs Abstract Classes

This week I also learned about abstract classes and found out they are pretty alike to interfaces. It isn't that clear to me when to use one or the other, but these are the similarities and differences I found:

|                Interfaces                |                                Abstract classes                               |
| :--------------------------------------: | :---------------------------------------------------------------------------: |
|     Interfaces cannot be instantiated    |                 Abstract classes cannot be instantiated either                |
|         They have no constructor         |                          They may have a constructor                          |
|    Can only implement other interfaces   | Usually can only inherit from one class but may implement multiple interfaces |
| By default, its methods are all abstract |        Has to have at least one abstract method to be an abstract class       |

It's worth mentioning that some years ago, only abstract classes could have some implemented methods, but nowadays, also interfaces may have implementations.



That's all for this week, bye!


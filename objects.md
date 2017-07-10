# Objects

Java is quite a class act. Java thinks everything is an Object! How classy of Java...

Last chapter you learned about the `int` and how to make variables.

Now for the most important part of Java: objects.

Java is an object-oriented language, which, as the name implies, means that Java is all about objects and their interactions.

Now what is an _object_?

This is going to get quite philosophical, so bear with me.

Think of objects in real life. Objects in real life have _states_ and _behaviors_. Take for example an apple - it's state is it's color, size, ripeness, etc. It's behaviors is be eaten, grow, die.

States are variable properties and behaviors are methods on which the object can be used.

Java takes this idea and implements it in code.

In software, an object's state is stored as _fields_ and it's behaviors are stored as _methods_.

![](https://docs.oracle.com/javase/tutorial/figures/java/concepts-object.gif)

For example, a Bicycle object in Java would have a couple of fields: mph, rpm, and it's gear. It's methods would include change gears, change cadence, and brake.

![](https://docs.oracle.com/javase/tutorial/figures/java/concepts-bicycleObject.gif)

Let's look at how a Bicycle class would be implemented in Java.


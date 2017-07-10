# Fields

Let's start with fields. Remember that fields represent a variable state.

Our `Bicycle` class should have 3 states: `rpm`, `mph`, and `gear`.

Luckily for you, you already learned how to do this!

Variables, when put inside of a `class` declaration, represent fields.

Using your knowledge of variables from a [previous chapter,](/variables.md) you can safely assume how to add fields to a `class`.

```java
public class Bicycle {
    int mph = 0;
    int rpm = 0;
    int gear = 0;
}
```

Cool! Let's test it out!

Go back to `HelloWorld.java`. Remember that all code starts from the `main` function. Your `main` function in `HelloWorld` should be empty, like this:

```java
public class HelloWorld {
    public static void main(String[] args) {

    }
}
```

To use your new `Bicycle` class, you use it as a variable.

Until now, you have only used `int`'s as data types. Remember that `int`'s are numbers. When you create a `class`, you can create a variable of that type. So lets create a new `Bicycle` variable called `foo`

```java
public class HelloWorld {
    public static void main(String[] args) {
        Bicycle foo;
    }
}
```

Cool! Now we can access it's fields using a dot `.`. To access it's `mph` field, you would type `foo.mph`. For example, we could theoritically do this:

```java
public class HelloWorld {
    public static void main(String[] args) {
        Bicycle foo;
        foo.mph = 5;//accessing the mph field and performing an operation on it
        System.out.println(foo.mph);
    }
}
```

The problem is that when you try to run this code it will give you the following error:

```
Exception in thread "main" java.lang.Error: Unresolved compilation problems: 
	The local variable foo may not have been initialized
	The local variable foo may not have been initialized

	at HelloWorld.main(HelloWorld.java:4)
```

We _declared_ a new variable called `foo` which is a `Bicycle`. However, `foo` doesn't have a value yet! We need to tell Java that we want a brand new `Bicycle.`

Luckily, Java was made for and by humans, so the syntax is pretty easy:

```java
Bicycle foo = new Bicycle();
```

The above line of code tells Java that the `foo` variable will be a new `Bicycle` object. We will learn about what the parenthesis are for a bit later.

Your code should look like this:

```java
public class HelloWorld {
    public static void main(String[] args) {
    	Bicycle foo = new Bicycle();
    	foo.mph = 5;
    	System.out.println(foo.mph);
    }
}
```

When you run it, it should print `5` to console. Congratulations! You just created your first real class!


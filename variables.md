# Variables

We want some action in Java! We want to do something! Printing stuff to console gets boring after a while.

Let's have some fun.

What kind of fun?

_Math_

Lets make our program print the answer to `2 + 2` to console.

Now, computers are great at math. In fact, computers know algebra!

![](https://imgs.xkcd.com/comics/applied_math.png)

If you are reading this tutorial, you are most likely in high school and have passed pre-algebra. If you haven't, I am concerned and you should totally understand pre-algebra before programming.

Remember back to the old days when you learned this:

$$a = 2, b = 3$$

$$c = a + b$$

This isn't a particularly hard algebra equation, but it's a great place to start.

Why are we relearning basic algebra?

All of programming relies on this algebra! Everything you will ever code requires algebra! In fact, code is just glorified math! You will see in a second.

Lets make our computer print out what `c` is from our algebraic expression.

For now, delete everything in your `main` function, so your `HelloWorld.java` should look like this:

```java
public class HelloWorld {
    public static void main(String[] args) {
    }
}
```

First, we need to create our variables, `a` and `b`.

Lets start with `a` first. We want the computer to create a new variable called `a` and give it the value of `2`. Easy enough, right?

```java
a = 2
```

Is probably what you would type in your `main` function. That is very close to the actual answer.

Remember from [one of the older chapters](/what-is-a-computer.md) when we talked about how computers are super dumb and literal? Here is your first example of that in action.

You see, variables obviously take up memory. Specifically data in your RAM. The computer needs to know how much space to reserve for variables in RAM. Not all variables take up the same amount of memory! For example, the number `3` takes up a lot less memory than the statement `Hello World`. Because of that, computers assign every variable a _data type._ A data type simply describes what kind of variable it is and what kind of data it stores.

The number `3` needs to have the data type of `int`. An `int` stands for the word integer. If you remember your algebra, an integer is a whole number. `3` is a whole number, thus it is an integer, and the computer needs to know that.

The specific syntax for creating a variable is like this:

```java
[type] [name] = [value]
```

From what we have talked about, the `type` of our variable is `int`, the `name` is `a`, and the `value` is `2`.

Putting 2 and 2 together \(get what I did there?\) leads us to this statement:

```java
int a = 2
```

That line creates a new variable that is an integer, called `a`, and has the value of `2`.

Lets do the same for `b` and put it in our `main` function

```java
public class HelloWorld {
    public static void main(String[] args) {
        int a = 2
        int b = 3
    }
}
```

We are forgetting one thing!

Java needs to know when a line ends. At the end of anything called a _statement_, you put a `;` \(semicolon.\) A statement is simply a line of code. You don't put semicolons after _blocks_ \(`{` and `}`.\)

[Here is a nice guide explaining what blocks and statements are.](https://docs.oracle.com/javase/tutorial/java/nutsandbolts/expressions.html)

In order for our code to work, you need to put a semicolon at the end of our lines of code, to do this:

```java
public class HelloWorld {
    public static void main(String[] args) {
        int a = 2;
        int b = 3;
    }
}
```

Now if you press the Run button...

...nothing will happen!

It seems like nothing will happen.

I promise you something did happen. It created 2 integers in your RAM, and gave them the values of `2` and `3`.

It didn't do anything with them, of course.

We need to now create our `c` variable, which will have the value of `a + b`.

Using our syntax to create variables, let's do it!

```java
public class HelloWorld {
    public static void main(String[] args) {
        int a = 2;
        int b = 3;
        int c = a + b;
    }
}
```

It is that easy! Computers are best at doing math, so obviously it would be built in.

To make sure our program works, let's print the value of `c` to console. It should print `5`.

```java
public class HelloWorld {
    public static void main(String[] args) {
        int a = 2;
        int b = 3;
        int c = a + b;
        System.out.println(c);
    }
}
```

\(remember to always put a semicolon at the end of every line of code!\)![](/variables/console-output)[Here is the official Java tutorial explaining variables](https://docs.oracle.com/javase/tutorial/java/nutsandbolts/variables.html). Look at it if you feel a bit confused!

![](https://imgs.xkcd.com/comics/purity.png)


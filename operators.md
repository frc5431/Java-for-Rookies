# Operators

In one of the [earlier chapters](/basic-syntax.md) I briefly mentioned expressions. I said that expressions involve a left and right value. Now we will expand on them!

Expressions consist of a left and right value plus an operator. An operator is simply a symbol that operates on 2 values. For example, in the expression `2 + 3`, the left value is `2`, the right value is `3`, and the operator is `+`. You have used a couple of operators already, like `+` and `=`.

## Math

Numerical primitives have the obvious mathematical operators: `+`, `-`, `*`, `/` for addition, subtraction, multiplication, and division respectively.

Note that a `double` plus a `double` equals a `double`, obviously. All of the operators result in the same type afterwards. Except for division. If you divide on whole numbers, aka non-decimal types, Java will automatically round down for you:

```java
int foo = 3 / 5;//the answer is 0!
```

In order to get the actual answer, you need to use one of the decimal types you just learned about:

```java
double bar = 3.0 / 5.0;//the answer is 0.6!
```

There is one other cool operator for use: modulo \(`%`\). Those who have taken Algebra 2 know what modulus does. But for those who don't a modulo operation is similar to division, except instead of returning the decimal result, it returns the remainder:

```java
double baz = 5.0 / 3.0;//baz is 1.6666666666666667
double bam = 5.0 % 3.0;//baz is 2 with modulo (2 remainder)

int laf = 26 % 10;//laf is 16 with modulo
```

Quick note: Java does not follow order of operations. Java does the math from left to right. You can use parenthesis `()` to specify operations to be done first:

```java
int math = 3 - (2 * 5);
```

## Assignment

You have used this operator a lot before: the `=` operator. This operator just assigns a value to something. Pretty simple.

You have always used it when creating a variable. You can also use it after the variable has been created, giving it a brand new value. Once you have created a variable, you don't need to say it's type again:

```java
int foo = 3;
foo = 5;//foo is now 5. didn't need to say its type - i've already created it!
```

However, when you are using primitives, you don't have to give it a value when you declare it! It will default to 0:

```java
int bar;//when you don't give it a value, it is 0 by default.
bar = bar + 1;//bar was 0, now it is 1.
```

This only works with primitives. With classes, you have to give them a value - usually with `new`.

You can also combine assignment with some math:

```java
//instead of
bar = bar + 1;
//you could do
bar += 1;//this adds 1 to bar.
bar -= 3;//this subtracts 3 from bar
bar *= 2;//this multiplies bar by 2
bar /= 2;//this divides bar by 2
```

Even cooler:

```java
bar++;//this adds 1 to bar.
```

## String operations

Believe it or not, you can add `String`'s.

Yep.

It's pretty easy actually:

```java
String impossible = "I don't understand how one could add ";
String newString = impossible + " strings!";
System.out.println(newString);//prints "I don't understand how one could add strings!"
```

You can add anything to a `String` and it will gracefully be converted exactly as you want it:

```java
String foo = "The answer is " + 42;//foo is "The answer is 42"
```

---

[Here](https://docs.oracle.com/javase/tutorial/java/nutsandbolts/operators.html) is the page with the official beginner's guide reference to operators. It defines a bunch of operators that you haven't learned yet - we will get to those as time goes on.

### Exercises

Head to the operating room and try playing around with the operators you just learned. Make the craziest mathematical expression you can think of print it to console! Your computer will always figure it out.

![](https://imgs.xkcd.com/comics/types.png)


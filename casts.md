# Casts

Variables may have given data types when they are created, but their values can change data types using casts.

```java
double foo = 3.0;
int bar = (int) foo;//bar has a value of 3 (int)
```

The above code is using a _cast_ to change the type of something. To cast a value, you put the new type in between `().`

However, casts aren't magic. They have rules to them. Do you think the following code is legal:

```java
double foo = 3.3;
boolean bar = (boolean) foo;
```

Spoiler alert: it is not! The second line, `boolean bar = foo;` is illegal because a `boolean` has to be `true` or `false`. `3.3` can't become `true` or `false` so obviously you can't cast it to a `boolean`!

What about this code:

```java
//is this code legal?
double foo = 3.3;
int bar = (int) foo;
```

The answer is: yes. The above code is legal.

But wait!

It has it's side effects. Remember, `int`'s can only store whole numbers, without decimals. `3.3` obviously has a decimal point! To make sure this cast works, the JDK will round it down, meaning `bar` will have a value of `3`.

All `int`-like types like `long`, `double`, or even `byte` can be cast to each other. However, remember there are memory limitations. The following code will work, but it may not have the intended effect:

```java
int foo = 300;
byte bar = (byte) foo;//a byte can only store values from -127 to 128. bar will "overflow"
System.out.println(bar);//prints 44
```

How did Java get from `300` to `44`? That is because it triggered something called an _overflow_. As the name implies, the number overflowed the max range of a `byte`, so it reset to it's minimum value of `-127` and continued from there.

---

Other than casting numerical types, you can cast anything to a `String`. That is how `System.out.println` is able to print anything!

---

[Here](https://docs.oracle.com/javase/specs/jls/se7/html/jls-5.html), [here](https://stackoverflow.com/questions/5289393/casting-variables-in-java), [here](https://howtoprogramwithjava.com/java-cast/), and [here](https://stackoverflow.com/questions/3001836/how-does-java-handle-integer-underflows-and-overflows-and-how-would-you-check-fo) are some great resources to read up more on casting.


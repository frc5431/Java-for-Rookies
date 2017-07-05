# Operators

Data types and variables are cool and all but we need to actually do something with them! Luckily for us, Java has a bunch of operators, or symbols that can perform operations on variables. Name is pretty self explanatory, huh.

## Math

Numerical data types have the obvious mathematical operators: `+`, `-`, `*`, `/` for addition, subtraction, multiplication, and division respectively.

Note that a `double` plus a `double` equals a `double`, obviously. All of the operators result in the same type afterwards. Except for division. If you divide on whole numbers, aka non-decimal types, Java will automatically round down for you:

```java
int foo = 3 / 5;//the answer is 0!
```

In order to get the actual answer, you need to use one of the decimal types you just learned about:

```java
double bar = 3.0 / 5.0;//the answer is 0.6!
```

## Assignment

You have used this operator a lot before: the `=` operator. This operator just assigns a value to something. Pretty simple.

You have always used it when creating a variable. You can also use it after the variable has been created, giving it a brand new value. Once you have created a variable, you don't need to say it's type again:

```java
int foo = 3;
foo = 5;//foo is now 5. didn't need to say its type - i've already created it!
```

In fact, you don't even need to give it a type when it's created:

```
int bar;
```




# If statements

The _if statement_ is the most basic control structure. It allows you to run code only _if _something is true.

```java
if(<condition>){
    <code>
}

//one line form
if(<condition>) <statement>;
```

[Remember when we learned about `boolean`](/data-types.md) and I told you that they have an important use?

Now you will learn that important use!

The `if` statement uses a condition to run a piece of code. A condition is either `true` or `false.`

```java
if(true){
    System.out.println("I will run!");
}

if(false){
    System.out.println("I won't run!");
}
```

However, you should never write `if(true)` or `if(false)`. That is just silly! You might as well use comments then.

The true power of the `if` statements is with a _logical operator _\([remember what operators are?](/operators.md)\)

Unlike mathematical operators, which operate on numerical types, and assignment operators, which operate on any variables, a logical operator operates on `boolean` values.

The simplest logical operator is the `==` operator. It compares 2 values and becomes `true` if they are equal, `false `otherwise:

```java
<value1> == <value2> // true if <value1> and <value2> are equal

int foo = 5;
int bar = 6;
int baz = 5;

foo == bar;//this is false, because 5 is not equal to 6
foo == baz;//this is true, because 5 is equal to 5
foo == foo;//this is also true, because anything is always equal to itself
```

Using this nifty operator, you can write `if` statements that change based on values in your code:

```java
int foo = 5;
int bar = 6;
int result = foo + bar;

if(result == 11){
    System.out.println("Math works correctly on this computer!");
}
```




# Data Types

Last chapter we learned about cool things called variables and how they all have data types. We learned about the `int` and how it represents an integer.

Every data type has strict rules surrounding how they can be used. For example, an `int` can only be a whole number. The following is not allowed:

```java
int foo = 3.3;//oops! 3.3 is a decimal, not a whole number!
```

In order to use decimals, there are 2 data types: `float` and `double`. Both allow decimals. A `double` is a decimal that is 64 bits \(8 bytes\) while a `float` is 32 bits \(4 bytes.\) Obviously, the more bits a number has, the more it can store. Roughly, a `float` can store about 6-7 numbers after the decimal point while `double` can store 15-16.

By default, any number you type with decimals will be a `double`.


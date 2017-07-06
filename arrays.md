# Arrays

Writing this book is a lot of work. I really need arrays...

---

Arrays are amazing ways for storing large amount of data. Arrays store a fixed amount of another type of variables.

Imagine that arrays are ways to store a collection of data. The syntax looks like this:

```java
dataType[] arrayName;//preferred way

dataType arrayName[];//works but not preferred
```

Here is an example declaring an array of `int`'s:

```java
int[] foo;
```

In order to properly create an array, you need give it a length. Arrays store a fixed amount of data. The syntax for creating an array looks like this:

```java
= new dataType[size];
```

To create arrays, you use a special new keyword - `new`. Making `foo` have a size of `10` would look like this:

```java
foo = new int[10];
```

So far, our code looks like this:

```java
int[] foo;//declare variable 'foo'
foo = new int[10];//give 'foo' value of an array of 10 ints
```

`foo` now contains 10 `int`'s inside of it. Sounds crazy!

The way you access the `int`'s inside of `foo` is with the `[]` operator:

```java
foo[3];//access 4th int in foo
```

That comment is not a typo. When you access an element inside of an array, you access it starting from 0 - meaning element 1 is accessed via `[0]`.

![](https://docs.oracle.com/javase/tutorial/figures/java/objects-tenElementArray.gif)

The reason we start at 0 is because of pointers and how arrays work from C/C++. All you need to know is that numbering starts from 0.

![](https://www.tutorialspoint.com/java/images/java_array.jpg)

Let's make `foo` have some values:

```java
foo[0] = 3;//element 1 at index 0 has a value of 3
foo[1] = 42;//element 2 at index 1 has a value of 42
foo[2] = -100;//element 3 at index 2 has a value of -100
```

Remember that the data type of `foo` is `int[]` meaning that it can only store `int`'s. You can make an array of any data type:

```java
boolean[] bar;
String[] baz;
```

In fact, you can even create arrays of arrays:

```java
int[][] mdArray;
```

This is called a multidimensional array. To create and access a multidimensional array, you simply add an extra set of `[]`'s to every operation you do:

```java
mdArray = new int[10][10];//create an array of 10 int arrays of size 10. it has 10 * 10 (100) elements overall

mdArray[0][0];//access element 0 of array 0 in array 0
mdArray[4][2];
```

---

Just like any other data type, there are also array literals. To create an array literal, you use the `{} `operator:

```java
int[] literally = { 1, 2, 3, 4, 5 };//create an array of 5 elements
```

The above code creates an array of 5 `int`'s and gives them values:

```
System.out.println();
```




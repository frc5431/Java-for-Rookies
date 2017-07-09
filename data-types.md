# Data Types

Last chapter we learned about cool things called variables and how they all have data types. We learned about the `int` and how it represents an integer.

Every data type has strict rules surrounding how they can be used. For example, an `int` can only be a whole number. The following is not allowed:

```java
int foo = 3.3;//oops! 3.3 is a decimal, not a whole number!
```

In order to use decimals, there are 2 data types: `float` and `double`. Both allow decimals. A `double` is a decimal that is 64 bits \(8 bytes\) while a `float` is 32 bits \(4 bytes.\) Obviously, the more bits a number has, the more it can store. Roughly, a `float` can store about 6-7 numbers after the decimal point while `double` can store 15-16. Additionally, a `double` is more precise doing math. Just like humans, computers round when they are dealing with large decimal numbers, so the more numbers after the decimal point, the less rounding that happens.

![](https://imgs.xkcd.com/comics/e_to_the_pi_minus_pi.png)

By default, any number you type with decimals will be a `double`. I personally recommend using a `float` whenever you can to save memory, but if you require accuracy and large decimals, always use a `double`.

[This Stack Overflow post ](https://stackoverflow.com/questions/27598078/float-and-double-datatype-in-java)can help explain the difference between `float` and `double` if you don't quite get it yet.

---

Another important data type to know is the `boolean`. A `boolean` is either `true` or `false`

What? No one said data has to be numbers!

```java
boolean foo = true;
boolean bar = false;
```

Why would you want to use a `boolean`? That will be explained later, young padowan, when we get to conditionals. Just remember it's existence...

---

There is another built in data type that isn't technically a number, and that is the `char`. A `char` stands for character and represents a single character of text. To represent a `char`, you put `'` \(single quote\) around a character, as so:

```java
//examples of chars
char foo = '4';
char bar = 'f';
char baz = '☭';//emojis are supported characters since Java 7!

char bam = 'hello!';//WOAH! you can't do that! char's are only single characters!
```

[If you remember back from when you wrote Hello, World](/our-first-program.md) you may remember seeing some double quotes. A double quote represents a `String` which is more than one character.

```java
String foo = "I am more than one character!";

String bar = '!';//can't do this, single quotes are for char, double quotes are for String
char baz = "I am so long!";//can't do this either, double quotes are for string
```

The values in between the `""` and the `''` are called literals.

```
Literals
```

A literal is basically a value that is hard written into the code. In our previous example,

```java
int a = 2;
int b = 3;
```

`2` and `3` are both integer literals. Whenever you type them in code, they will always be an `int`. There are literals for any type.

For example, `3.3` is a `double` literal. It's type is `double`. To make it a `float` literal, you put the `f` at the end, making it `3.3f`.

```java
double foo = 3.3;//3.3 is a double literal
float bar = 3.3f;//3.3f is a float literal

float baz = 3.3;//oops! 3.3 is a double, not a float!
```

`true` and `false` are literals for `boolean`

Double quotes `"` are literals for `String` while a single quote `'` is a literal for a `char`.

Additionally, a number prefixed with `0x` is a hexadecimal value \(something you really don't need to know\) and a number prefixed with `0b` is pure binary.

## Every primitive data type

The data types we just went over are called _primitives._ They are data types built in to Java. We can create our own data type using _classes_, something we will go over soon. There are couple of other primitives not mentioned previously because they are a bit less important. You don't have to know every single small detail about every single data type. The following is a reference for the future.

| Primitive Name | What it stores | Example\(s\) of a literal | Size in memory |
| :--- | :--- | :--- | :--- |
| int | A whole number \(no decimals\) from  -2,147,483,648 to. 2,147,483,647 | 42000000 or hexadecimal \(0x280DE80\) | 32 bits \(4 bytes\) |
| short | A whole number from -36,768 to 32,767. Basically a smaller int. | 1337 | 16 bits \(2 bytes\) |
| byte | A whole number \(no decimals\) from -128 to 127. Basically an even smaller int. | 42 or binary \(0b00101010\) | 8 bits \(1 byte\) |
| long | A whole number \(no decimals\) from -9,223,372,036,854,775,808 to 9,223,372,036,854,775,807. A very huge int. Use this for big numbers. | 999999999999L or 999999999999l | 64 bits \(8 bytes\) |
| float | A decimal number with a range of 3.40282347 x 10^38 to 1.40239846 x 10^-45. Has roughly 5-6 decimal places. Less precise than a double | 3.3f | 32 bits \(4 bytes\) |
| double | A decimal number with a range of 1.7976931348623157 x 10^308 to 4.9406564584124654 x 10^-324. More precise than a float. Has roughly 15-16 decimal places. | 5.6 | 64 bits \(8 bytes\) |
| boolean | Either true or false. Used in conditional statements. | true or false | 1 bit |
| char | A single character of text. Otherwise equivalent to a short except it doesn't go into negatives \(0 - 65,535\) | 'a' or \u0041 | 16 bits \(2 bytes\) |
| String | Collection of chars. Basically text. | "Hello, world!" | Variable length. Depends on length of text. |

Here is an example showing every type of literal:

```java
int a = 42;
int b = 0x2A;//42 in hexadecimal
short c = 12;
byte d = 21;
byte e = 0b00010101;//21 in binary
long f = 99999999999L;
float g = 5.6f;
double h = 3.1459;
boolean i = true;
boolean j = false;
char k = 'a';
char l = \u0041;//'a' as a unicode code point
String m = "I am quite literally a literal!";
```

Here are some references about data types if you need a bit more understanding:

[http://cs.fit.edu/~ryan/java/language/java-data.html](/h ttp://cs.fit.edu/~ryan/java/language/java-data.html)

[https://docs.oracle.com/javase/tutorial/java/nutsandbolts/datatypes.html](https://docs.oracle.com/javase/tutorial/java/nutsandbolts/datatypes.html)

### Exercises

Feeling fearless? Try to create a variable of every data type using your literals and print it out to console! Try seeing what it prints.


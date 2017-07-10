# Basic Syntax

There are a couple of basic syntax rules and vocubulary that all Java code has.

## Comments

Comments are ignored by the compiler and allow you to basically take notes on your code. We went into detail about comments on [this page](#comments).

## Statements

Statements are basically lines of code. A statement is similar to a sentence in English grammer: it is a series of words that forms a complete sentence. A single statement forms a single instruction for Java to execute.

There are 3 types of statements: expression, declaration, and control flow statements.

```java
int variable;//declaration statement

variable = 5;//expression

if(variable == 5){
    //control flow statement
}
```

There will be pages about each statement in detail later on. For now, just remember that every type of statement has to end in a semicolon `;`.

## Expressions

Just line in math, an expression is an operation that has a _left_ and a _right_ value that evaluates to a single value.

```
//examples of expressions:
variable = 5;
5 + 5
2 * 3
"Hello " + " world!"
array[0] = true;
```

You will learn about what each of these expressions do as time goes on. For now, remember that expression always has a left and right value.

Notice that some of the above expression examples have semicolons. Those are _expression statements_, one of the first type of statements we just talked about! Yay!

## Blocks

Blocks are combinations of statements surrounded by curly brackets `{` and `}`. Remember from our Hello World example, the `main` function and the `HelloWorld` class have curly brackets. Those are examples of blocks!

---

Always remember to put a closing curly bracket `}` and semicolons `;`. A missing semicolon or bracket are annoying to track down!

![](https://i.redd.it/gpgc6u4cglyy.jpg)

If you want a little more reading to understand, [here is the official guide explaining this topic.](https://docs.oracle.com/javase/tutorial/java/nutsandbolts/expressions.html)


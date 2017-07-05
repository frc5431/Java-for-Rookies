# How does this program work?

Here is the program again:

```java
public class HelloWorld {

    public static void main(String[] args) {
        // Prints "Hello, World" to the terminal window.
        System.out.println("Hello, World");
    }

}
```

The beauty of this program is that it shows a bunch of concepts vital to Java. It can really be split into 4 different sections:

![](/first-program-explanation/overview.png)

## Class declaration

The class declaration creates a new class called `HelloWorld`. A class \(not to be confused with a `.class` file\) is an object in Java. Every file has a class in it. We will talk about classes later, but just know for now that every `.java` file has a class in it with the same name. To create a class, you type the word `class` and then it's name.

Notice those curly brackets? The `{`? That is called a scope. Each time you write a `{`, you must put a `}` to end it somewhere else in the program. In the case of our class above, everything written in between the first set of  `{` and `}` belongs to the class `HelloWorld`.

## Main function declaration

Next is the main function declaration. We will talk about functions specifically in more detail later. This function has a name - `main`. The `main` function in this case belongs to the `HelloWorld` class because it is in between the curly brackets for `HelloWorld`. The function has it's own set of curly brackets - this is where you write actual Java code. Functions allow you to run code. Everything in between the function's curly brackets will be run by `main`.

When you run your Java program, the JVM will find the `main` function and run that first. Think of `main` as the entry point to your program, or the start of it. Everything begins there. The `main` function always has to look like this:

```java
public static void main(String[] args)
```

An explanation of what all of that means will come later. For now, just remember that the `main` function is where your program starts.

## Single line comment

This is called a single line comment. Comments are ignored by the JDK and provide no actual functionality. They only exist to write notes to help yourself or other programmers understand the code. There are 3 forms of comments:

```java
// Single line comment. Whenever the // is encountered, the rest of the line is ignored
/* Multiline comment. Everything after the /* is ignored. Even
stuff on new lines. The way to end multiline comments is by
writing */
/** Documentation comment. This is identical to the multiline comment, except it is intended
for documenting your code using JavaDoc. That is outside the scope of this tutorial, but
it is highly recommended you use documentation after you finish this tutorial.
To end it, you simply write */
```

Think of a comment as just that - it is a small note written by a human to explain something or comment about something. The compiler just ignores it. Comments can go anywhere in the program - even outside of your class declaration. In the case of our program, the comment explains what the next line does - print "Hello, World!" to the terminal window.

![](https://imgs.xkcd.com/comics/commented.png)

## Print statement

This is where the magic happens. Remember we briefly talked about functions? `System.out.println` is a function. Functions allow you to run other code. In this case, the `System.out.println` function takes in input and puts it in your console window. The action of \_printing \_means to put something onto the console.![](/first-program-explanation/console.png)Anything you put in between the parenthesis will be put in your Eclipse console tab. In fact, lets experiment! Try replacing `"Hello, World"` with `4.2` and watch what happens.![](/first-program-explanation/changing-println)Now `4.2` was printed to console instead!

![](https://www.commitstrip.com/wp-content/uploads/2016/12/Strip-Lignes-de-commande-english650-final-2.jpg)

Try experimenting with this. Try multiple println statements even!


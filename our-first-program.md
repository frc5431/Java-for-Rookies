# Our first program

Lets actually jump to business and actually write a Java program! It won't do anything flashy or control a robot yet, just something to make sure everything works.

As per tradition, your first program is the \_Hello World \_program. Every programmer starts off with the Hello World program!

First, lets create a simple Java project:

![](/first-program/new-project.png)

Call your project "HelloWorld" and click Finish

![](/first-program/project-name.png)

Your Eclipse should look like this:![](/first-program/eclipse-view.png)If you are still on the start page, click the X button next to where it says "Start Page"

On your left, you can see your new HelloWorld project. If you collapse it, you should see a folder called `src` and your JRE. `src` is the folder where all of your code will go. It stands for _source_.

Lets create a new Java class. For now, think of classes as individual files. Right click on `src` and add a new class.

![](/first-program/add-new-class.png)

Call your class HelloWorld and click Finish![](/first-program/hello-world-class-created.png)Sweet! We have our first class. We can write the HelloWorld program. Copy and paste this code into HelloWorld.java:

```java
public class HelloWorld {

    public static void main(String[] args) {
        // Prints "Hello, World" to the terminal window.
        System.out.println("Hello, World");
    }

}
```

Now click the big green run button to run this program.![](/first-program/big-green-button)If everything worked correctly, a new tab at the bottom called "Console" should have appeared and say the text `Hello, World`![](/first-program/console-hello-world)If your Eclipse doesn't look like this, you did something wrong. Try to look carefully and retrying some of the previous steps to get it to look like this. [This link](https://docs.oracle.com/javase/tutorial/getStarted/problems/index.html) has a couple of common problems found when compiling Java for the first time. If you need help, ask one of the coders on programming team. We are here to mentor you in case you need help!

[Here is the official Java getting started tutorial.](https://docs.oracle.com/javase/tutorial/getStarted/index.html) It's really useful! It does a couple of minor things slightly differently than the way I do it, but in the end, it also results in a Hello World program. Check it out if you feel lost or just want to solidify your learning.

![](http://www.commitstrip.com/wp-content/uploads/2013/09/Strips-Hello-world-600-finalenglish.jpg)

You just did a bunch of things and you probably have no idea what is going on. We will go slowly and explain everything that just happened and what you just did.


# Compiler vs Interpreter

Lets go step by step and explain everything as it comes along. I just mentioned the interpreter, which is the secret sauce that makes Java work with any food.

Interpreters and compilers both achieve the same purpose - to turn this:

```java
public class HelloWorld {
    public static void main(String[] args) {
        // Prints "Hello, World" to the terminal window.
        System.out.println("Hello, World");
    }
}
```

into this:

```nasm
.text                           # section declaration

                                      # we must export the entry point to the ELF linker or
    .global _start              # loader. They conventionally recognize _start as their
                                      # entry point. Use ld -e foo to override the default.

_start:

                                # write our string to stdout

      movl    $len,%edx           # third argument: message length
      movl    $msg,%ecx           # second argument: pointer to message to write
      movl    $1,%ebx             # first argument: file handle (stdout)
      movl    $4,%eax             # system call number (sys_write)
      int     $0x80               # call kernel

                                # and exit

      movl    $0,%ebx             # first argument: exit code
      movl    $1,%eax             # system call number (sys_exit)
      int     $0x80               # call kernel

.data                           # section declaration

msg:
    .ascii    "Hello, World!\n"   # our dear string
    len = . - msg                 # length of our dear string
```

> What's the difference?

The second one \(look how ugly it is\) is called _assembly_. You have probably heard of this term. Assembly is what your computer understands to make things happen. Assembly is the closest thing a human can write in to how a computer actually works that isn't binary. Binary would be almost impossible for any human to code in!

Assembly is still very difficult. Look how ugly it is! And it's super complicated to do a simple thing. Of course, it has it's advantages. It is super fast and gives you the most control of the computer. But which would you prefer? The 6 lines of clean code at the top or the much longer ugly code at the bottom?

I hope you prefer the top one. Because that is Java, which is what you will be learning very soon!

The problem is, computers don't understand Java. They only understand assembly. In fact, every processor has a different type of assembly they like! When you write assembly, you can basically only write it for one model of computer. Obviously, there is a quite a problem here. How do we turn our nice, clean code into assembly?

## Tada! Compilers are here!

Some nerd decided to make a _compiler_. The first compiler was written in assembly and it turns non-assembly into assembly. Let's  take GCC for example. GCC is a compiler for the C programming language. When you run GCC, it turns C code into assembly for a target computer, and then into binary for the computer to run. For every processor type, you have to run GCC to generate an executable file for it.

That's why a .exe on Windows doesn't run on Mac - it's different assembly code!

In order for your C program to run on both Windows and Mac, you have to use GCC to compile it to the two different executable types. That doesn't mention the hundreds of distributions of Linux!

That doesn't sound that bad until you realize that compilations of big programs can last a long time, even _hours_ to build some of the most popular applications from scratch. And these include millions of lines of code, a bunch of other libraries, huge scripts to run commands. It's crazy!

![](https://imgs.xkcd.com/comics/compiling.png)

It does get very tedious. That's the problem with compilers - they can take a long time to compile and they have to be run separately for every platform.

[Here is a nice video explaining compilers](https://youtu.be/o-xSgi9o5vk)

## Move aside - interpreters are here!

One day, in 1958, Steve Russel realized that he could make a program run code instead of compiling it. He promptly wrote the Lisp Interpreter, which will \_interprets \_a Lisp script and runs it without compiling.

![](https://imgs.xkcd.com/comics/lisp_cycles.png)

The idea is pretty simple - instead of compiling every program for every computer, you compile 1 program that can run other programs.

The advantages for an interpreter is that it works anywhere - as long as you have the interpreter on your system, you can execute scripts. Examples of interpreted languages are Javascript, Lua, and Python. In order to run this scripts, you have to have the interpreter on your system. This is one of the downsides of interpreted languages - you must download the interpreter on every system you want to use it on. Also, interpreted languages are slightly slower than compiled languages because the interpret has to run your script very quickly. It doesn't have time to make optimizations like a compiler does.


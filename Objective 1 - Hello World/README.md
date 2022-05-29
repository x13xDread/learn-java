# Objective 1 - Hello World

Welcome to the first objective of the course! In this objective we will get you off and running with the very bare bones basics for writing Java code. This Objective relies on you having completed the instructions in the README.md file in the main directory of this repository. This includes setting up your workstation with a debugger and installing Java. If you have this done then lets get started!

## Hello World
The first lines of code we are going to write are vare simple. We are going to write a simple Java program that prints out the words "Hello World" to the console.

```java
public class HelloWorld {
    public static void main(String[] args) {
        // Prints out "Hello World" to the Console
        System.out.print("Hello World");
    }
}
```

Now this looks kind of overwhelming at first as there is a lot going on here. But we can break it down into a few steps. On the first line we have written:
```java
//the file name matches the class name
public class HelloWorld {
```
`Public Class` is reffering to something later on that we will learn about called classes but for now its important to know that the class is what holds our java code together. `HelloWorld` is the name of the class and is also the name of the file. When you do an exercise later in this module you will want ot make sure your class name matches the file name otherwise it will not work. This is one of the common sources of errors for beginners. 

You will also have noticed that there is a `{` after the name of the class. This is where the code starts. Likewise there is a matching `}` at the end of the class. This `}` is where the code stops. All your code will be contained in the brackets of both the class and the pair of brackets on the next line.

```java
    public static void main(String[] args) {
```
Here we see something kind of similar to what was on the first lineof the code but very different. whats important to know here for now is that this is where all of the code you want executed goes. In later objectives I will show you what this means in more detail. For now remember to include this and the matching brackets before writing out your code.

```java
    // Prints out "Hello World" to the Console
```
Next is this Green line that doesn't really look like code. That's because it isn't! This is a comment and its used by developers to explain what their code does both for their own benefit and for that of others. Everyone will pick up their own style for writing code and proper documentation in larger projects can save time of having to read through lots of code to understand what it does.
```java
    System.out.print("Hello World");
```
This is the code we are using to print to the console. Lets break it down. Firstly we have the word `System`. It wasn't mentioned earlier but note the capitilization. Java is case sensitive when it comes to naming things so its important that when trying to write code you always use the same capitalization. `System` refers to exactly what you think it would, the System or Operating System your computer runs on.

Next is `.out`. The leading . before the word out means we are accessing a part of the `System` (in this case `out`) and likewise after `out` we see another leading period with `.print` meaning that we are accessing a part of `out`. `print` again does exactly what you think it would do, print some words. You'll notice after `print` there is a `(` and a `)` and these are the arguments, or in this case words, that we are passing to `print` to print out to the console. Here you see that we are passing the words `"Hello World"` to be printed. 

Its important to note that the words that you want to print must be surrounded by quotes. This is so Java knows that these are letters and not java code. Without the quotes Java will be confused and think that the words are java code causing it to throw an error. Later we will see how we can pass in other arguements to the `print`.

The very last but super important thing to note is that after the parentheses there is a `;`. This is used to end the line of code and is very important. It is essentially the same as ending a sentence with punctuation. This semicolon tells the debugger that the code on this line is done and that it can move on to the next line.

To see what our code does we can now run it in our terminal. You can copy and paste the code above into a .java file or run the code provided in the examples folder in Objective 1. Depending on what you set your workstation to do this may be different but if you are using VSCODE you can run your code by using the keyboard shortcut `ctrl + f5` on windows or by going to `run > run without debugging`.
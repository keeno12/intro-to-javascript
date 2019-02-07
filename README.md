# Learn to Code: Introduction to JavaScript

Brought to you by Galvanize. Learn more about the way we teach code at [galvanize.com](http://galvanize.com).

Get to this repo by typing in URL:

## Overview
The goal of this brief course is to provide you with a fun introduction to the world of web development with Javascript.

#### Here's what we'll be doing:
* Overview of basic JavaScript concepts
* Building a simple application using javascript
* Playing around and break things


#### What is programming?
Programming is giving your computer a set of instructions to perform a task.

This sounds simple but it can get complicated!


## Setting up your computer


#### Please set up the following:

* A web browser to see what we're working on as others see it (Recommend Google Chrome: [chrome.google.com] (http://chrome.google.com))
* We will be using an online text editor for this workshop. You can sign up here: [https://repl.it/](https://repl.it/)


Well... that was easy!


## What this workshop is

A super friendly introduction to JavaScript No previous experience expected!

You can't learn EVERYTHING in ~2 hours. But you can learn enough to get excited and comfortable to keep working and learning on your own! Come to our almost weekly code hours [events](https://www.galvanize.com/sanfrancisco/events/) to ask questions if you get stuck and show off what you've been working on!

- This course is for absolute beginners
- Ask Questions!
- Answer Questions!
- Help others when you can
- Its ok to get stuck, just ask for help!
- Feel free to move ahead
- Be patient and nice


## About me:

Hello I'm Keenan Olsen. I'm a Technology Evangelist here at Galvanize! Previously I've worked at IBM and on numerous projects in web development. I'm from Boulder, CO where I went to the University of Colorado Boulder.

- Twitter: [@KeenanOlsen](https://twitter.com/@keenanolsen)
- LinkedIn: [Keenan Olsen](https://www.linkedin.com/in/keenanolsen/)
- Email: [keenan.olsen@galvanize.com](mailto:keenan.olsen@galvanize.com)


## About you!

Give a quick Intro!

- Whats your name?
- Whats your background?
- Why are you interested in JavaScript?

## What is javaScript?

### A very brief history

Created by Brendan Eich in 1995 in ONLY 10 days during his time at Netscape Communications.

A lot of updates have happened of course since then, but its still fun to see some of the [quirks](https://www.destroyallsoftware.com/talks/wat) still in the language!

Read more about the history of JavaScript [here](https://en.wikipedia.org/wiki/JavaScript).

Javascript is often used with HTML and CSS to create dynamic web pages.

### Who uses javaScrip?

Almost everyone!

- Large Companies (Google, Facebook)
- Startups
- Agencies
- Pretty much anyone using web technology


### What can you do with JavaScript

- Web Development
	- Front-End
	- Back-End
- Mobile Development
- [Machine learning](https://js.tensorflow.org/) 😱
- [Embedded(Hardware) Programming](http://ejs.co/) 😲

#### Popular Frameworks to keep in mind

When learning more about JS you'll probably keep learning about these!

- Node
- Express
- React
- Angular
- Vue


## JavaScript Basics:

### Data Types:
We're going to stick with the basics, so We wont be going over EVERY data type in javascript, but you you can read a more comprehensive list [here](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Data_structures).  

Feel free to try these code samples out in your developer console(I'll show you how) or your repl!

#### Numbers:

Numbers are written just like you would think. Just the number! No quotes or symbols to worry about. If you do put quotes around a number it will become a string (see next)

`25` `100`

Multiple, Add, Divide, Compare

- `5 * 5` | output: 25
- `5 + 5` | output: 10
- `8 / 2` | output: 4
- `8 > 2` | output: true

#### Strings:
Strings can be a collection of letters, symbols and/or numbers. They are made by surrounding the content with quotation marks.

`"Hello, World."`
`"CrAzy Random String 987879896jvdjvda &&(&(@*(*"`

Can we add strings together? Try it out!


#### Booleans:
You can think of Booleans as yes(true) and no(false)

`true` `false`

We'll go into how to use these in a little bit. For now just remember they exist!


## Variables:
Variable are a way to store information.
This is super useful! You can then receive or update the variable in your program. You'll see this later!

Think of it as naming a piece of data.

We're going to define our variable using the keyword `var`. Its very common to see variables not defined using the newer keywords `let` or `const`. We won't go into the differnces in this workshop but you can read more about `let` & `const` [here](https://medium.com/javascript-scene/javascript-es6-var-let-or-const-ba58b8dcde75). For now just remember that `var` means we're creating a new variable.


- `var twitter = "@KeenanOlsen";`
- `var score = 0;`


## Comparison Operators:
Comparison Operators are used quite frequently in programming. Its a great way to compare and use data.

Again we won't cover ALL of the comparison operators in this workshop, but you can see a full list of them [here](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators)

- `==` Equal
- `===` Strict Equal
- `!=` Not Equal
- `>` Greater Than
- `>=` Greater Than or Equal
- `<` Less Than
- `<=` Less Than or Equal

Example:

`current_score >= highest_score`
This would return a boolean value. Depending on the values of these variables this would return either `true` or `false`. Try it in your console using numbers instead of variables!


## Functions
Reduce, Reuse, Recycle

Functions make it easy to reuse code. If you find yourself repeating code you may want to turn it into a function!

Example:
This function takes in two arguments(a, b) and returns the value of them added together.

```
function add(a, b) {
	return a + b;
};
```
to use the function call it by writing its name and open/close parenthesis(). With arguments passed inside the parenthesis():

- `add(5,5)` | output: 10
- `add(2,5)` | output: 7

In this simple example you're not saving a ton of code, but imagine a function that uses many lines of code!


## Conditionals

When writing a program you'll often want to check if data meets a certain condition or not. We can use conditionals to make decision about our data and create different outcomes

 In javascript you'll often use the `if` statement. This may be followed by `else if` or `else` depending on how many conditions need to be checked.

Example:

```
if (guess == answer) {
    message = "You Win!";
} else if (guess < answer) {
    message = "Your guess is too low!";
} else if (guess > answer){
    message = "your guess is too high!";
} else {
	message = "I think you entered something wrong...";
}
```

## Loops
We're going to go over some of the basic loops in javascript, but yet again we're not going to cover everything, so you may want to read more about loops [here](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Loops_and_iteration).

Loops are used when you want to repeat something. You can repeat the exact same thing, or change some variable and repeat the action again.

two common types of loops are `for` and `while`.
`for` loops are often used to run a loop a specified amount of time.

`while` loops are often used to run a loop indefinitely until certain criteria are met.

Example:

This `for` loop will run 5 times, and print out the value of `i` to the console.

```
var i;
for (i = 1; i <= 5; i++) {
    console.log(i)
}
```

If `i` were set to 1 it would run this loop and print the string until the value of `i` changed. If you run this in your browser it will probably crash it!

```
var i = 0;
while (i == 1) {
    console.log("I will crash your browser")
}
```


## Interact with dialog boxes
using dialog boxes can be simple way to get started interacting with users.

Alert: Pop up information in a dialog box

`alert("Hello, I'm a pop up");`

Prompt: get information from a user in dialog box

`prompt("I'm a pop up you can type in!")`


## Lets do some code!
You just learned a lot! Lets put it together and build something!

Sign up if you haven't already and create a new project: https://repl.it/


We're going to build a number guessing game using:

- variables
- Comparison Operators
- Conditionals
- loops
- functions
- dialog boxes

If you get stuck or want to look ahead at the completed project you can view it [here](https://repl.it/@SageElliott/GuessingGame).

What are some ideas for improvements?

- Exit on command
- data validation
- input the number range from popup
- output grammar depending on number of tries


# YOU DID IT! YOU'RE NOW A PROGRAMMER!

### Welcome! :)

### Keep learning!



## What is Galvanize?
###### We are a community!


## Relevant Upcoming Events at Galvanize

We host sooo many events! check out out [calendar](https://www.galvanize.com/sanfrancisco/events)

- [Learn to Code Workshop: Intro to Machine Learning](https://www.meetup.com/SF-Data-Science/)

- More Learn to codes coming soon!!!

- [Data Science](https://www.galvanize.com/sanfrancisco/data-science)
- [Software Engineer](https://www.galvanize.com/sanfrancisco/web-development)


#### Co-working Space
[work in our building!](https://www.galvanize.com/entrepreneur)


## Questions:
Please feel free to reach out to Sage Elliott with any questions!

- Twitter: [@keenanolsen](https://twitter.com/@keenanolsen)
- LinkedIn: [KeenanOlsen](https://www.linkedin.com/in/keenanolsen/)
- Email: [keenan.Olsen@galvanize.com](mailto:keenan.olsen@galvanize.com)

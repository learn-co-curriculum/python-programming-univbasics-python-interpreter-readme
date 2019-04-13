# Introduction to Python Interpreter

## Learning Goals

1. Define the Python interpreter
2. Identify REPLs
3. Explain why REPLs are useful
4. Access and exit the Python interpreter via your terminal
5. Execute commands in the Python interpreter
6. Demonstrate the typographical convention for showing return values in-line
7. Demonstrate the typographical convention for offsetting code

## Introduction

So, we're ready to have a conversation with Python. We can't very well open up a
computer and start talking to it.

![Engineer Montgomery Scott Attempts Communication with a 20th Century
Computer](https://media.giphy.com/media/3o7btVRbshbbaC8Ygg/source.gif)

Instead, we run a program that's a "conversation room." In it we send
_expressions_ for Python to _evaluate_. After Python evaluates the _expression_,
it will send back _return values_, or responses.

## Define Python Interpreter

The Python interpreter is like a room specially built for having conversations
with Python. We can think of it as your Python playground. The Python
interpreter is run from within your computer's terminal by typing `python`. Once
the Python interpreter is running, we key in Python _expressions_ and hit ENTER.
Afterward we'll see Python's evaluation of the _expression_ (the _return
value_).

Programs like the Python interpreter are known as "REPLs." "REPL" stands for
_Read–Evaluate–Print Loop_. Many languages feature REPLs: Python, Ruby, Lisp
and others. We'll talk more about REPLs in the next section.

> **IMPORTANT**: The Python interpreter is _not_ a file where you save your
> work. Any coding you do in the Python interpreter will not get saved. It only
> exists temporarily. The Python interpreter is for testing and playing with code.

## Identify REPLs

REPL stands for read–eval–print loop.

If you think about it, that's what you do when you're being the listener in a
conversation.

You:

1. "read" in the other person's expression ("I'm curious about learning programming!")
2. "evaluate" what the expression means ("My friend is bored at their job? My friend wants to make more money?)
3. "print" your reponse ("Oh great!" "I love programming, you're going to love it too!").

The Python interpreter, as a REPL, gives you a place where:

1. _You_ type in a Python expression (which the Python interpreter "reads")
2. The _Python interpreter_ "evaluates" the expression based on the rules of Python
3. The _Python interpreter_ "prints" a response or a _return value_

## Explain why REPLs are useful

Sometimes we want to see how code works. Instead of having to build a brand new
program (in a file), load up all the libraries, blah, blah, blah, the Python
interpreter is a quick "laboratory" where we can see how something works. This
is usually better than looking at the docs or writing a Stack Overflow post.
With just a simple bit of test data we can _verify_ we understand how a line of
code is working.

Think about a car: it's a complex machine with many interacting parts. But if
your car won't start you might "isolate" the battery and hook it up to a
battery tester. If the battery tester shows the battery is good, then you know
that the problem is somewhere else; if the battery is dead, then you have
_verified_ that the battery is the problem with your car.

That process is known as _debugging_ when applied to computers or
_troubleshooting_ when applied to pretty much everything else. At the risk of
sounding mystical, debugging is a skill shared by all makers: guitarists to
brewers, to chefs, to programmers. From Neal Stephenson's _Cryptonomicon_:

> Randy counts four men in addition to Amy and the pilot...  All of them are
> fiddling around with engines or diving gear in a way Randy recognizes,
> through many cultural and technological barriers, as debugging.

## Access and Exit the Python Interpreter Via Your Terminal

To access the Python interpreter, just type `pyhon` in the terminal. Let's start
by typing a few _expressions_ into the Python interpreter and see the
read-evaluate-print-loop for ourselves.

### Instructions

1. Open up a terminal. You can launch the Learn Sandbox and use the terminal at
   the bottom.

2. Type `python` and hit `return`

3. Now that you've started the Python interpreter, type the commands below to
see how it works! Type each of the following lines into the Python shell and
press enter.

- `255 / 5`
- `9 ** 2`
- `print("hello world")`

To leave the Python interpreter, type the `exit()` command - this will get you
back to your command line.

### Session Example

![Example Python Interpreter
Session](https://curriculum-content.s3.amazonaws.com/programming-univbasics/Python Interpreter-readme/Python Interpreter-readme.gif)

### Reflecting on Conversation

Congratulations! You've had a conversation with Python! Python is a good
conversationalist and waits for you to issue an _expression_. Python _evaluates_
this expression and returns its interpretation of your expression: a _response_
or _return value_.

For `Time.now`, Python looks at your computer's clock and _returns_ the time. For
`255 / 5` it evaluates your expression's use of the division _operator_ (more
on them later) and does some mathematics to produce `51`. Similarly, the `**`
means "use what comes after me as an exponent to what's in front of me" and
returns `81` (it's the same as 9<sup>2</sup>).  Lastly, the `puts`
expression means "print something, in this case, `hello world`.

### Typographical Conventions

#### Showing Return Value

As you saw in that last section, it was kind of annoying to read the return
values as separated from their _expression_. When it's helpful, Pythonists like to
document a return value _next to_ its expression with `#=>`.

The `#` in Python is a comment character and everything after it is ignored. The
`#=>` is simply a tool to help you "imagine" what Python Interpreter might do with the
expression.

Python documentation frequently looks like:

- `Time.now #=> 2019-03-26 14:00:27 -0400`
- `255 / 5 #=> 51`
- `9 ** 2 #=> 81`
- `puts "hello world" #=> nil`

> **NOTE**: That `puts` returns `nil` is a very interesting and mildly strange
> thing to see, but it's true. We'll talk all about it later.

If you wanted to put one of these examples in Python Interpreter, you'd copy up to the `#=>`
but _not_ include it (or anything after it until the end of the line).

#### Offsetting Code

Whenever we're writing a word of Python code or a value that Python returns we put
it in `this typeface`. So while "9 times 9 is 81", `9 * 9 #=> 81`. This
convention should make code things "pop out" for your eye.

## Conclusion

As we get into more complex code, sometimes we need a quick scratch pad to work
in to test a bit of code out. Python Interpreter is great for this purpose. We can use it to
learn about unfamiliar keywords, calculate equations, and, in general, become
more comfortable writing in Python.

# Introduction to IRB

## Objectives

1. Define IRB
2. Identify REPLs
3. Explain why REPLs are useful
4. Access and exit IRB via your terminal
5. Execute commands in IRB
6. Demonstrate the typographical convention for showing return values in-line
7. Demonstrate the typographical convention for offsetting code

## Introduction

So, we're ready to have a conversation with Ruby. We can't very well open up a
computer and start talking to it.

![Engineer Montgomery Scott Attempts Communication with a 20th Century
Computer](https://media.giphy.com/media/3o7btVRbshbbaC8Ygg/source.gif)

We run a program that's a "conversation room." In it we offer _expressions_ for
Ruby to _evaluate_ and to which it will offer _return values_, or responses.

## Define IRB

IRB stands for "Interactive Ruby." It's a like a room especially built for
having conversations with Ruby. Programs like IRB are known as "REPLs." IRB is
run from within your computer's terminal.

IRB is _not_ a file where you save your work. Any coding you do in the IRB
console in your terminal will not get saved anywhere. It only exists
temporarily. IRB is for testing, playing, manipulating your code so that you
understand it better and solve problems with it.

## Identify REPLs

REPL stands for read–eval–print loop.

If you think about it, that's what you do when you're being the listener in a
conversation.

You:

1. "read" in the other person's expression ("I'm curious about learning programming!")
2. "evaluate" what the expression means ("My friend is bored at their job? My friend wants to make more money?)
3. "print" your reponse ("Oh great!" "I love programming, you're going to love it too!").

IRB, as a REPL, gives you a place where:

1. _You_ type in a Ruby expression (which IRB "reads")
2. _IRB_ "evaluates" the expression based on the rules of Ruby
3. _IRB_ "prints" a response or a _return value_

## Explain why REPLs are useful

Sometimes we want to see how code works. Instead of having to build a brand new
program (in a file), load up all the libraries, blah, blah, blah, IRB is a
quick "laboratory" where we can see how something works.

Think about a car: it's a complex machine with many interacting parts. But if
your car won't start you might "isolate" the battery and hook it up to a
battery tester. If the battery tester shows the battery is good, then you know
that the problem is somewhere else; if the battery is dead, then you know right
what to do.

That process is known as _debugging_ when applied to computers or
_troubleshooting_ when applied to pretty much everything else.

> Randy counts four men in addition to Amy and the pilot...  All of them are
> fiddling around with engines or diving gear in a way Randy recognizes,
> through many cultural and technological barriers, as debugging.

From Neal Stephenson's _Cryptonomicon_

## Access and Exit IRB Via Your Terminal

To access IRB, just type `irb` in the terminal. Let's start by typing a few
_expressions_ into IRB and see the read-evaluate-print-loop for ourselves.

### Instructions

1. Open up your terminal. (If you do not have a terminal on your computer you
   can use [repl.it][repl])

2. Type `irb` and hit `return`

3. Now that you've started IRB, type the commands below to see how it works!
   Type each of the following lines into the IRB shell and press enter.

- `Time.now`
- `255 / 5`
- `9 ** 2`
- `puts "hello world"`

To leave IRB, type the `exit` command - this will get you back to your command line.

### Session Example

![Example IRB
Session](https://curriculum-content.s3.amazonaws.com/programming-univbasics/irb-readme/irb-readme.gif)

### Reflecting on Conversation

Congratulations! You've had a conversation with Ruby! Ruby is a good
conversationalist and waits for you to issue an _expression_. Ruby _evaluates_
this expression and returns its interpretation of your expression. For
`Time.now`, Ruby looks at your computer's clock and _returns_ the time. For
`255 / 5` it evaluates your expression's use of the division _operator_ (more
on them later) and does some mathematics to produce `51`. Similarly, the `**`
means "use what comes after me as an exponent to what's in front of me" and
returns `81`.  Lastly the `puts` expression means "print something, in this
case, `hello world`.

### Typographical Conventions

#### Showing Return Value

As you saw in that last section, it was kind of annoying to read the return
values as separated from their _expression_. By convention, Rubyists sometimes
document a return value _next to_ an expression as separated by `#=>`.

The `#` in Ruby is a comment character and everything after it is ignored. The
`#=>` is simply a tool to help you "imagine" what IRB might do with the
expression.

In our example we would write:

- `Time.now #=> 2019-03-26 14:00:27 -0400`
- `255 / 5 #=> 51`
- `9 ** 2 #=> 81`
- `puts "hello world" #=> nil`

> **NOTE**: That `puts` returns `nil` is a very interesting and mildly strange
> thing to see, but it's true. We'll talk all about it later.

If you wanted to put one of these examples in IRB, you'd copy up to the `#=>`
but _not_ include it (or anything after it until the end of the line).

#### Ofsetting Code

Also whenever we're writing a word of Ruby code or a value that Ruby returns we
put it in `this typeface`. So while "9 times 9 is 81", `9 * 9 #=> 81`. This
convention should make code things "pop out" for your eye.

[repl]: https://repl.it/

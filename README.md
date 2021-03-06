# Assignment 1: Collatz

## Introduction

The goal of this assignment is to introduce you to the basics of OCaml
programming and apply them to some simple problems.

## Part 1: Online Tasks
- Register for our [Ed discussion board](https://us.edstem.org/join/WKvVTz).
    When you have a question about a problem set, Ed will be your go-to source.
- Read the introductory notes on
    [Functional Basics](https://www.cs.princeton.edu/courses/archive/fall22/cos326/notes/basics.php)
    and
    [Type Checking](https://www.cs.princeton.edu/courses/archive/fall22/cos326/notes/type-check.php).

## Part 2: Setting up your Development Environment

Check out the course resources web site for help
[getting starting with OCaml](https://www.cs.princeton.edu/courses/archive/fall22/cos326/resources.php)
and installing or configuring a development environment for your chosen editor,
such as emacs, vim, VS Code, or atom. Once you have OCaml installed and your
development tools set up, now you just have to learn how to write useful
programs!

## Part 3: Assignment Basics

You should see the following files in this repository:
- `a1.ml:` The main file for your assignment. Look inside the file to find a
    series of short problems you should solve.
- `testing.ml:` A file with the tests that will be used to evaluate `a1.ml`.
- `signature.txt:` You will record your sources here.

You can compile `a1.ml` by typing:

```
$ ocamlbuild a1.native
```

This will do two things. First, it creates the executable file `a1.native`.
Second, it creates a directory called `_build` full of auxiliary files used by
the OCaml compiler system. To run the executable we have created, type:

```
$ ./a1.native
```

If you haven't touched any of the code inside `a1.ml` yet, you should see the
following message printed out:

```
Fatal error: exception Failure("undefined")
```

That indicates the `Failure` exception has been raised. Follow the instructions
in `a1.ml` to eliminate the error and complete the assignment.

To delete the `_build` directory and remove the executable files you have
created, type

```
$ ocamlbuild -clean
```

This assignment asks you to answer the questions contained within the `a1.ml`
file. Make sure the entire file type checks and compiles before you hand it in.

## Important notes

1. **Compilation errors:** Your solution *must compile*. If you omit problems
    (you shouldn't!), leave the corresponding definitions commented out so that
    they will not confuse our automated grader as it checks the other problems.
    If you are having difficulty getting your code to compile, please visit
    office hours!
2. **Testing:** We have provided tests for most of the functions you will write
    in `a1.ml`. In order to run these tests, compile with
    `ocamlbuild testing.native`, and run the resulting executable.
3. **Auxiliary functions:** Feel free to use them when they make your code
    cleaner, more modular, and/or easier to test &mdash; that's what functions
    are for! Just make sure that if we name a particular function that you have
    to write (either in the assignment text, or in a template file), that you
    preserve its name so that our automated grader can find it.
4. **Style:** Finally, please pay attention to style. Take the extra time to
    think about the problems and find the most elegant solutions before coding
    them up. Many of the problems in this assignment are somewhat artificial.
    Nevertheless, think about your coding style where appropriate (and
    certainly, thinking about style in the final question computing pi is
    appropriate). For reference, consult the
    [COS 326 style guide](https://www.cs.princeton.edu/courses/archive/fall22/cos326/style.php)
    and the
    [lecture notes](https://www.cs.princeton.edu/courses/archive/fall22/cos326/schedule.php).
    In addition, you are also encouraged to bring style questions to the course
    staff at office hours.
5. **Line limit:** One important element of style is having at most 80
    characters per line. This is important for our ability to read your code.

## Hand In

Your assignment will be automatically submitted every time you push your changes
to your GitHub repository. Within a couple minutes of your submission, the
autograder will make a comment on your commit listing the output of our testing
suite when run against your code. **Note that you will be graded only on your
changes to `a1.ml`**, and not on your changes to any other files.

You may submit and receive feedback in this way as many times as you like,
whenever you like, but a substantial lateness penalty will be applied to
submissions past the deadline.

We will give you some indication that you have not drastically misinterpreted
the specification by checking if your solution compiles. These are not tests,
make sure to use the tests in `testing.ml`.

It is **very important** that you compile and test your code while in your Git
root directory. These steps will check that your code as a whole compiles and
that the tests pass. Using the interactive toplevel REPL for typechecking is
very useful but **is not sufficient** for these purposes. Submissions that do
not compile will earn very few points!

Start early! Work hard!

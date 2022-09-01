# Assignment 1: Collatz

## Introduction

The goal of this assignment is to introduce you to the basics of OCaml
programming and apply them to some simple problems.

## Part 1: Online Tasks

- You should be already automatically registered for our [Ed discussion board](https://edstem.org/us/courses/25177).
    When you have a question about a problem set, Ed will be your go-to source.
- Read the introductory notes on
    [Functional Basics](https://www.cs.princeton.edu/courses/archive/fall22/cos326/notes/basics.php)
    and
    [Type Checking](https://www.cs.princeton.edu/courses/archive/fall22/cos326/notes/type-check.php).

## Part 2: Setting up your Development Environment

Check out the course 
[Resources page](https://www.cs.princeton.edu/courses/archive/fall22/cos326/resources.php) and 
install opam, ocaml, and VS Code (or some other editor of your
choice).  Once your development tools are set up, now you just have to
learn how to write useful programs!

## Part 3: Assignment Basics

You should see the following files in this repository:
- `a1.ml`: The main file for your assignment. Look inside the file to find a
    series of short problems you should solve.
- `signature.txt`: You will record your sources here.

After you clone the repo, create a Unix terminal window (inside VS Code, or outside VS Code if you like), make sure it's in the right directory.

You can run `a1.ml` by typing:  `ocaml a1.ml`.

Either way, if you haven't touched any of the code inside `a1.ml` yet, you should see the
following message printed out:
```
Exception: Failure("undefined")
```

That indicates the `Failure` exception has been raised. Follow the instructions
in `a1.ml` to eliminate the error and complete the assignment.  That is, edit in VS code, save your file, then `ocaml a1.ml` until everything works.  In the process, you may find it helpful to use the read-eval-print-loop (REPL)

## Running inside the ocaml read-eval-print-loop

Save your file; from your terminal shell prompt, type `ocaml` or `utop` and at the `#` prompt, type `#use "a1.ml";;`  This will let you interact with your program, as demonstrated in lecture or precept.

## Important notes

1. **Compilation errors:** Your solution *must compile*. Submissions that do not
    compile will earn very few points! If you omit problems (you shouldn't!),
    leave the corresponding definitions commented out so that they will not
    confuse our automated grader as it checks the other problems. If you are
    having difficulty getting your code to compile, please visit office hours!
2. **Testing:** How should you write tests? At some point during the semester,
    we may talk about testing in more depth than you saw in the first lecture.
    For now, we will mostly leave testing up to you (though please follow the
    instructions in the file and write some tests where we ask). Follow the good
    practices you have learned in earlier COS courses.
3. **Auxiliary functions:** Feel free to use them when they make your code
    cleaner, more modular, and/or easier to test&mdash;that's what functions are
    for! Just make sure that if we name a particular function that you have to
    write (either in the assignment text, or in a template file), that you
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
5. **Line limit:** Please use no more than 80 characters per line, so
    we can read your code and we're in a better mood when we grade it.

## Hand In

Your assignment will be automatically submitted every time you push your changes
to your GitHub repository. That is,

```
$ git commit -a -m "Message identifying your commit, for your own convenience"
$ git push
```

Within a couple minutes of your submission, the autograder will make a
comment on your commit listing the output of our testing suite when
run against your code. You can read this comment in github, and you'll
also get it in e-mail.

**You will be graded only on your
changes to `a1.ml` and `signature.txt`**, 
and not on your changes to any other files.

You may submit and receive feedback in this way as many times as you like,
whenever you like.

Start early! Work hard!

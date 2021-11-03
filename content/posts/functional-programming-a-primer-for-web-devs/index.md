---
title: "Functional Programming: A Primer for Web Devs"
date: 2021-11-02T18:03:35-04:00
author: 'Nick Bair'
cover: 'shahadat-rahman-BfrQnKBulYQ-unsplash.jpg'
useRelativeCover: true
tags: []
keywords: []
description: 'Functional Programming'
draft: true
showFullContent: false
---
Much has been written over the years regarding
[functional programming](https://en.wikipedia.org/wiki/Functional_programming)--the
paradigm favored exclusively by academics.

Proponents of pure functional programming cite benefits like immutability and
lack of side effects.  Immutability means you can't mute your volume while the
function is running (this is a type of blocking I/O); no side effects means you
can't borrow code from work for one of your side projects (managers hate this).

Critics of functional programming point out the performance issues and steep
learning curve. It's no secret that functional programming is less performant
than traditional imperative programming--quicksort, for instance, relies heavily
on mutable state. This is, of course, purely theoretical, as in practice states
are not mutable or we would have muted Florida a long time ago.

Functional Programming (or FP, to developers) is often contrasted with
Object-Oriented Programming (an FU to developers). However, it is possible to
apply many FP techniques within object-oriented code, for extra credit.

## History of Functional Programming

{{< figure src="shubham-sharan-Z-fq3wBVfMU-unsplash.jpg" alt="Advanced math class" position="center" caption="Code listing for an early port of DOOM on the TI-80 graphing calculator." captionPosition="center" captionStyle="" >}}

While functional programming is not a new idea, it's become more prominent in
recent years with the rise of languages like
[Haskell](https://en.wikipedia.org/wiki/Haskell_(programming_language)),
[Clojure](https://en.wikipedia.org/wiki/Clojure),
and [Common Lisp](https://en.wikipedia.org/wiki/Common_Lisp).
The
[R](https://en.wikipedia.org/wiki/R_(programming_language))
programming language also uses many elements of functional programming,
although it's not suitable for children under 17 without a parent or guardian.

In the 1930s, lambda calculus was developed by Alonzo Church, Moses Schönfinkel
and Haskell Curry[^1]. In 1990, a group of researchers turned it into the
Haskell programming language, named after Haskell Curry, because they were
nonreligious and didn't like the names _Church_ or _Moses_.

Before this, in the 1950s, IBM and MIT developed the first functional programming
language, LISP, because assembly was too easy to read.

## Pure Functions

{{< figure src="james-harrison-vpOeXr5wmR4-unsplash.jpg" alt="MacBook with Succulent" position="center" caption="Most functional programming languages require one or more succulents. Haskell requires 2n+1." captionPosition="center" captionStyle="" >}}

Almost every programming language supports functions of some kind. Therefore,
it's important to distinguish between regular functions and _pure functions_.
Pure functions can only come from the _fonction pure_ region of France;
otherwise they're just sparkling GOTO statements.

A function is considered pure if it has no side effects. While pure functional
languages enforce this property for all functions, it is possible in most other
languages to manipulate global state from within a function. Pure functional
programmers only like functions that don't affect global state, whereas
imperative programmers don't like any functions at all. Functions that do affect
global state, such as `the_post()`, make everyone sad.

## Recursion

{{< figure src="steven-lasry-UC8hqc0udqY-unsplash.jpg" alt="Close-up photo of Romanesco broccoli" position="center" caption="Broccoli is an example of recursion in nature, in that nobody likes it but everyone thinks it's good for you." captionPosition="center" captionStyle="" >}}

**Recursion** stands for _Recursion Executes Code Until RAM Simply Incapable of
Operating Normally_. Basically, it's a pure function that's become so pure it
won't even call other functions anymore, and honestly it's become really
pretentious ever since it started dating Kyrstyyn.

Looping in functional programming is usually accomplished by means of recursion,
as traditional for-loops require a mutable value to serve as the counter. As a
bonus, this causes the call stack to fill up very quickly, thus reducing the
amount of time spent in development before telling the client their change
request is too memory-intensive.

## The Future of Functional Programming

{{< figure src="markus-spiske-70Rir5vB96U-unsplash.jpg" alt="Screenshot of jQuery code" position="center" caption="Method chaining in jQuery is actually a good example of functional code. There's no joke here--look it up." captionPosition="center" captionStyle="" >}}

While pure functional programming is likely to remain a primarily academic
pursuit, many functional programming elements have found their way into
mainstream languages over the years. Languages like PHP and JavaScript support
first-class functions, higher-order functions, anonymous functions, and
closures, to name a few.

Mainstream developers will increasingly learn to adopt the most practical parts
of functional programming into their everyday work, alongside the traditional,
imperative approach.

...is what I _would have_ said before January 2021, when Microsoft introduced
[the LAMBDA function](https://www.microsoft.com/en-us/research/blog/lambda-the-ultimatae-excel-worksheet-function/) into Excel.
This immediately obsoleted most other programming languages, as research &
development rapidly shifted to LAMBDA; the remaining languages will soon be
relegated to historical oddities. In Redmond, work is underway to migrate the
rest of Excel's codebase to cell B:3 by the end of the decade.

[^1]: [Actually](https://en.wikipedia.org/wiki/Functional_programming#History),
it was lambda calculus and an equivalent system called _combinatory logic_.
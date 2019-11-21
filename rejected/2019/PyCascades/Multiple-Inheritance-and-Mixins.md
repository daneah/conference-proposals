# Multiple Inheritance and Mixins

## Abstract

If you’re like me, your class hierarchies may be getting out of hand.
Inheritance has proven hairy and now your code is giving you headaches.
Composition may be good for what ails you!
Come see how this works in Python and add another tool to your belt for cleaning up your code.


## Description

At the advent of object-oriented programming, inheritance and the class hierarchy reigned supreme.
You could model _anything_, from `Animal` all the way down to `Animal` -> `Mammal` -> `Dog` -> `UtilityDog` -> `FrenchBulldog`.
Eventually this got out of hand.

Today, composition brings many of the benefits of complex inheritance while keeping functionality focused and isolated.
In many languages, composition is achieved via the interface pattern; an object can declare its intent to implement a particular interface and as a result is beholden to support the behaviors that interface outlines.
In Python, there is no such thing as an interface!
What do we do about that?

Fortunately, Python provides the ability to support something interface-like (and more) via multiple inheritance.
In multiple inheritance, an object may inherit from multiple other objects.
Let’s explore how this works, what pitfalls to look out for, and how not to repeat the past when dealing with class hierarchies.


## Notes

* Old-style vs. new-style classes (5 minutes)
* `__init__`, `super()`, and inheritance refresher (6 minutes)
* Multiple inheritance example and pop quiz (5 minutes)
* Method resolution order (6 minutes)
* The Mixin pattern (5 minutes)
* Recap and tips (3 minutes)

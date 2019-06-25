# Code is a Liquid

## Abstract

We write code to provide solutions for business requirements.
Business requirements can change quickly and frequently, but code needs to change even more often.
We often treat existing code as something special because of the time and effort we've invested in it, but this isn't sustainable.
Code needs to be malleable in order to adapt to a continuously changing landscape.


## Details

### Who

This talk is for intermediate-to-advanced Python developers who would like to improve their understanding of refactoring and software architecture.
Attendees should have a working knowledge of classes and inheritance.
This will resonate most with folks who (want to) work in a collaborative environment, reading and writing code with others.

### Takeaways

After attending this talk, folks should have a good understanding of the terminology used to talk about code qualitatively as well as a few specific tools for addressing rigid code in Python.

### What

As projects age and grow, some areas of code—especially those rarely visited—harden into something that's difficult to work with.
Entropy manifests as complicated conditionals, long methods, and big classes, which in turn encourage more of the same.
It can be easy to feel frustration or despair at the thought of fighting off code rot.
Recognize that real-world projects all experience this phenomenon in one way or another, and that continuous, incremental improvement is a sustainable strategy.


## Outline

* Properties of liquids (3 minutes)
    * Particle arrangement
    * Cohesion
    * Viscosity
    * Take the shape of their container
* Encountering solid code (3 minutes, 6 total)
* What is "liquid" code? (10 minutes, 16 total)
    * Separation of concerns
    * Cohesion, encapsulation and loose coupling
    * Viscosity and extensibility
* Approaches and tools in Python (10 minutes, 26 total)
    * Separation of concerns into methods, classes, modules
    * Inversion of control
    * Delegation
* Recap and closing (4 minutes, 30 total)
    * _Introducing_: the LIQUID principles

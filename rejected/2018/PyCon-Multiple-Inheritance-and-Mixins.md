# Multiple Inheritance and Mixins

## Description
You've likely been using class inheritance for some time in your Python, whether you realize it or not.
Class inheritance may not be as great as millions-of-dollars-from-your-estranged-second-cousin's-uncle inheritance,
but it's exceedingly useful. We'll explore inheritance briefly before moving on to multiple inheritance.
You'll learn what multiple inheritance is, what benefits it has, and what pitfalls to look out for.
Once we've covered how multiple inheritance works, we'll run through a few real-world examples
that show how powerful an abstraction they can be.

## Audience
This talk is targeted at beginning and intermediate Python users who would like to understand multiple inheritance
as well as real-world cases where they are or are not an appropriate approach.

Audience should have a clear understanding of the general concept of inheritance as a foundation for multiple inheritance.
Afterward they should have a deeper understanding of multiple inheritance, its benefits, and its caveats.

## Outline
- Introduction (2 minutes)
- Refresher on class inheritance
  - Classes inherit from `object` in Python 2 (the default in Python 3) (2 minutes)
  - How `super()` works (5 minutes)
- Introduction to multiple inheritance
  - Syntax (2 minutes)
  - Method resolution order and resolution of `super().__init__(self)` (7 minutes)
- Examples
  - Toy example to show what to expect (2 minutes)
  - An authentication mixin in Django (5 minutes)
- Conclusion, key takeaways (2 minutes)
- Questions (3 minutes)

## Additional notes
If accepted, this would be my first conference talk!
I've presented technical content to audiences of 10-50 people in the past for internal purposes.
I've written blog posts on [Easy as Python](easyaspython.com) and have code available on [GitHub](github.com/daneah).

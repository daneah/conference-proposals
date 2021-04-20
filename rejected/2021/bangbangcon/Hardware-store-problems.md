# Hardware (store) problems: Lessons learned from debugging physical systems

## Description

A year ago I joined the 60%+ of Americans who have embarked on the journey of home ownership. In the ensuing months I’ve found out just where I fall on the spectrum between MTV Cribs and The Money Pit.

Though I haven’t encountered any critical structural issues, I have uncovered a myriad of opportunities for improvement. Each of these little “joys” of home ownership has served as a lesson in solving problems, and we’d be remiss not to heed these in writing and debugging our Python software.

## Audience

This talk is geared toward developers who want to improve their systems thinking skills. Attendees will want to know how they can build safer applications that interact in an ecosystem of other applications, and they'll come away with a framework for problem solving that can be applied across a variety of scenarios. The desire to write safer software isn't tied inherently to a particular experience level, but may correlate with intermediate-to-advanced attendees.

## Outline

### Introduction (1 minute)

* Setting the stage—we bought and renovated a home
* About me

### Know the modes of problem solving (2 minutes)

* Things are on fire (prod issues)—put it out immediately
* Creating new value (features)—how could things become on fire?
* Tech debt (bugs)—how on fire is it?

### Consider costs and benefits (5 minutes)

* There are often different solutions—each has ups and downs.
* Writing our own code or using an existing package have differing levels of control, maintenance burden, speed of iteration, and experience gain.
* Whereas homes appreciate in value, code typically depreciates.
* When you do decide to solve a problem yourself, do the research up front. You may not get it perfect, but it will be a workable solution.

### Generate hypotheses (5 minutes)

* Some problems are straightforward, but most aren’t obvious at first glance.
* Use observations to drive hypotheses. Throw out assumptions.
* Think about all the players—assume they’re flawed. Do the work to prove each part of the system is, in fact, working. Use new observations to support and refute hypotheses.

### Provide test points (5 minutes)

* Observability helps us understand system health—lack of observability is lack of evidence.
  * Emit logs and metrics for core workflows and put them in front of eyes.
  * Observed shifts in metrics can indicate systemic shifts in behavior.
* Testability is observability—if you can test something readily, it has observable behavior.
  * Invert control to increase flexibility.
* Some things just aren’t yours to know—proprietary systems will force your hand. Remember this during your cost / benefit analysis!
  * Particularly frustrating with leaky abstractions—you can see where the problem comes from, but can’t see how to fix it or see that it can’t be fixed.

### Uncover similarities and differences (3 minutes)

* Understanding a problem is often about reducing the search space.
  * Use hypotheses to discount systems from consideration.
* “Works on my machine!”—Understand the similarities and differences between two configurations to uncover the genesis of issues.
  * Same Python + pip versions?
  * Same package versions?
  * Same git commit?
  * Same environment variables?
  * git-bisect can help.

### Build in safety nets (5 minutes)

* Even when code has the right behavior, it can run suboptimally.
  * Noisy pipes
  * Leaky faucets
  * Flickering lights
* Provide ways to take a system offline for maintenance.
  * Feature flags are great for iterative development.
* Provide ways to automatically shed load on a system.
  * Retry stampedes can take down a service.
  * CircuitBreaker pattern and backoff logic can help.
* When in doubt, fail obnoxiously. Fail silently only if things are at an acceptable level of on fire and you have a backup plan.

### It’s adapters all the way down (2 minutes)

* Software seeks to convey or convert data—functions and systems adapt a domain to a range.
  * Useful in algorithm development—example: cosine/sine map (-inf, inf) to [-1, 1]
* Seek to reduce entropy at each step (robustness principle).

### Conclusion (2 minutes)

* Solve problems scientifically.
* In the absence of science, solve problems flexibly.
* Some fires are okay, but put them out eventually.
* We have the power of automation—run regression tests automatically on a schedule or with each change.
* Code will still degrade—dust quarterly and prune dead bits regularly.

# Elevating the engineering experience with Click, Textual, and universal design

## Abstract

Growing your engineers means giving them the space to choose tools that are best for solving a problem in the moment and learning. Over time, successful patterns emerge, but cruft sticks around too. Left unchecked, each engineer might end up with a bespoke set of notes and aliases and scripts about how to do a variety of things in a variety of contexts and often fumbles to remember how to accomplish a particular task.

From a management perspective, this looks like low productivity or ineptitude. How might we frame this instead as a systems problem and use good design principles to understand user needs and produce something valuable to veteran and new staff alike?

## Description

At ITHAKA, over 100 engineering staff manage hundreds of applications in a handful of languages and frameworks. Regardless of the details, development on an application often requires a particular set of similar tasks.

We work on JSTOR, a website serving millions of users globally. Keeping the systems behind JSTOR running is no small feat, and as we continue to build new value it gets just a _little bit_ tougher to maintain what's already built. Efficiency is key.

As we looked to continue doing more with less, we realized some of our frequent common tasks were being accomplished using one-off scripts, divergent approaches, and hope. Even when we'd create an official offering, without constant exposure many engineers would forget to use it, or forget about its existence altogether.

Taking cues from others in the industry building developer tooling, we imagined what it could look like to offer a single entry point command with a discoverable set of features. This tool would be _the_ place to go to accomplish common tasks.

This talk will cover lessons learned in designing such a tool, using Click and Textual to accomplish the interface, and how it all worked out in the end.

## Outline

- Background
  - About ITHAKA
  - About JSTOR
  - About operational efficiency
- Challenges
  - Many empowered teams on a deadline
    - Plus many tasks to accomplish
    - Creates many ways of doing things
  - Innersource model
    - Empowers anyone to contribute
    - But diffuses ownership
    - Leading to less communication and "stickiness" of solutions
- Can we build something that sticks?
  - Needs to accomplish the same tasks
    - But better
    - And in less time
    - While creating a feeling of supportedness
- Universal design principles
  - Affordances
  - Signifiers
  - Designing for accessibility to the least empowered of your audience
- Building the thing
  - CLI with Click
    - Commands and subcommands
    - Options and arguments
    - Help text
  - TUI with Textual
    - The composition model
    - Widget choices
  - Bonus: a blend with Trogon
  - Testing strategy
  - Rollout and adoption
  - Creating healthy contribution
- Helping us help ourselves
  - Tracked with Sentry early on to identify user challenges
  - Built in an automatic check for new versions and a command to upgrade
- Outcomes
  - Metrics TBD
  - Culture TBD
- (Meta) Learnings
  - CLI design tips
  - TUI design tips
    - Snapshot testing
  - Productive development tips

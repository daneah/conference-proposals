# One tox to rule them all: Orchestrating the Python packaging lifecycle

## Description

When you land in an existing project you’ve never seen before, it can be overwhelming. You need to wade through the sea of configuration files and commands to write, document, package, install, run, and test the code. Maintainership also requires a lot of interpersonal effort, so at the end of the day additional friction caused by the code and tooling can start to wear you down.

Creating a consistent interface as an entrypoint to most maintenance activities can reduce the strain of day to day activities. Using a tool that handles some of the heavy lifting of packaging by default takes this relief a step further. tox supports a wide area of the packaging lifecycle, and you can use it for great good in making your own software a breeze to maintain.

## Audience

Those who author and maintain several Python packages, or want to reach that point, would benefit from a consistent experience across their catalog. This makes it easier to document processes, reduces cognitive load, and empowers more of the team to carry out maintenance activities. All of this allows teams to focus on the value they want to deliver instead of the peripheral activities.

This talk will help attendees understand the tox philosophies of multiple environments with their own dependencies that execute specific tasks, going on to show how this can be used not only for the usual activity of testing but also formatting, linting, documentation, and application execution.

## Outline

### Salutations (1m)

### Maintainership is hard (5m, 6 total)

* Each tool has its own configuration file and command (2m)
* Documentation efforts often fall short and don’t cover contributing workflows (1m)
* Dependency management (2m)

### What could make this all easier? (5m, 11 total)

* Package-first testing to verify deliverables, not source code (2m)
* Inspired by npm: a single entrypoint to multiple, optionally interdependent tasks (1m)
* Transparent dependency management (1m)
* A single configuration file (1m)

### Enter tox (8m, 19 total)

* Tox environments (2m)
* Tox dependency management (2m)
* Tox command specification (2m)
* Breaking down some example tox commands (2m)

### tox translates to continuous integration workflows, too (4m, 23 total)

* Tips for using tox in Travis CI + Jenkins (3m)
* We fixed a tox + Jenkins bug! (1m)

### Conclusion (5m, 28 total)

* One portal to the management of a project (1m)
* venvless management (1m)
* Highly bootstrappable (live demo of creating a bootstrapped package project from a cookiecutter) (3m)

### Q&A (2m, 30 total)

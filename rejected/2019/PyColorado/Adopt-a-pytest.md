# Adopt-a-pytest

## Abstract

`pytest` is a testing framework that makes writing and running Python tests simpler.
Adopting new tooling in a large system is often a burden.
How can you introduce `pytest` gradually with minimal pain?


## Details

### Who

This is for anyone currently using `unittest` for Python unit testing that would like to adopt `pytest`.

### Takeaways

* How to run `pytest`
* How to create a basic `pytest` configuration
* Using `pytest` marks to shim an existing project
* Converting a `unittest` test to `pytest`

### What

With its simplified syntax, powerful fixture behaviors, detailed test reports, and plugin-based architecture, `pytest` has a lot to offer.
Whether you're new to Python unit testing or you've been using `unittest` for a while, `pytest` may be something to consider.
It's not too hard to get up and running with `pytest` on a fresh project, but how can you retrofit an existing project without having to refactor the world all at once?


## Outline

* Overview of `pytest` (5 minutes)
    * Syntax
    * Test discovery
    * Fixtures
    * Plugins
* Swapping in `pytest` (8 minutes, 13 minutes total)
    * Removing existing test runners
    * Running `pytest`
    * Using a fixture as a shim
    * Broad test collection
* Embracing `pytest` (8 minutes, 21 total)
    * Simplifying a `unittest` test
    * Removing a fixture shim
    * Speeding up/cleaning up test collection
* Some great plugins (3 minutes, 24 total)
* Recap and closing (1 minute, 25 total)

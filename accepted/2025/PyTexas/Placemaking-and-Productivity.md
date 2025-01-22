# Place-making and productivity: Build maintainable broad-scale tools with a small team

## Abstract

As we bring on new team members, we want to ensure they can ramp up quickly and have a good experience.
They should be able to understand "the company way" of accomplishing things and quickly find the tools they need to do their job.
Veteran team members should also be able to codify and commoditize the patterns they've developed over time so they can focus on higher-order problems.

In large organizations, such tooling might be the purview of a dedicated platform engineering team and have a budget to match.
But what if you're a small team, or a team of one, and you want to build something that scales to the whole organization without becoming a full-time job?

At ITHAKA, over 100 engineering staff manage hundreds of applications in a handful of languages and frameworks across many teams and products.
Despite the variety, most of those engineers still need to perform a core set of tasks when developing, from debugging to traffic routing to feature toggles.

Teams are always working on high-priority projects, and it can be difficult to find the time to take stock of things that can be better streamlined or automated.
Further, although we have a platform engineering team, as a non-profit we don't have the budget for someone to work on meta-tooling as a full-time job.
Over time, several aspects of our development process have become common sources of friction, with a lot of time spent answering questions or debugging local machine setups.

In this talk I'll tell the story of my journey to build a tool with a net positive return on investment, from the initial idea to the rollout and adoption.
I'll cover the principles that guided my decisions, the tools we use, and the outcomes we've seen so far.

## Description

Python developers have been creating command-line interfaces for years, and the ecosystem continues growing with tools like Typer, Rich, and Textual.
These tools help create a great user experience between the invocation of a command and its output, but there's a lot that happens before, during, and after that moment.
Engineers need to discover the tooling, download and install it, and understand what features it offers (note: some of them may have never touched Python before!).
When they run a command, the tooling needs to provide feedback to users and report errors to maintainers.
Over time, the usage of the tooling needs to be tracked and analyzed to understand how it can be improved.
Throughout, engineers need to feel supported and empowered to use the tooling effectively.

I'll cover the initial proof-of-concept of the tooling, starting with a Click-based CLI, and the evolution over time to a suite of tools supporting a well-oiled machine for engineers:

- Typer
- Trogon
- Rich
- Textual
- pipx
- Sentry
- CI/CD
- `importlib`
- `packaging`
- Dynamic plugins

This setup has allowed a small team of five to build and maintain a tool suitable to the needs of over 100 engineers, with very little reactive maintenance and fully asynchronous support.
Recently, new tooling is being added to the CLI first, making it *the* place to go to get things done.

I'll also cover building a supportive community around the tooling, including:

- Contribution guidelines
- Slack communication
- GitHub issues and pull requests
- Documentation
- Observability

Finally, I'll cover some delighters we've added to the tooling for a well-rounded CLI experience:

- Command aliases
- HTML-based help
- Automatic update notifications
- Diagnostic commands

My hope is that you'll come away with newfound inspiration to build internal tooling at your organization where you previously thought it insurmountable.
If you're already maintaining a suite of tools, I hope you'll find some new ideas to improve your process and outcomes.
I'd consider it a smashing success if I can learn something from your experiences in follow-up conversations!

## Notes

Some of the other maintainers of the tooling may co-present with me, depending on their availability and interest.

## Outline

- (2m) Introduction
  - Who I am
  - Who I work for
  - What we do
  - Why I'm here
- (5m) The problem
  - Our team structure and architecture
  - The friction points
  - What we needed to do
  - Previous attempts and challenges
- (10m) The solution
  - (2m) The initial proof-of-concept
  - (3m) The evolution of the tooling
  - (4m) How we achieved different aspects
    - Discovery
    - Installation
    - Understanding the tool
    - Upgrades
    - Plugins
    - Observability
    - Community and support
  - (1m) The delighters
- (3m) How it's going
  - Adoption rate
  - Open questions and challenges
- (5m) Q&A

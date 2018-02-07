# From Many Repos to Monorepo

## Abstract
As an organization grows, bits and pieces of its code base sprout up organically in different repositories.
At some point along the way, this model may stop making sense and start causing more harm than good.
How do we reign this in, and what are the pitfalls along the way?

Come learn about the pitfalls we experienced when our code was split across many repositories,
how we went about bringing it into a single repository, and the new pains and benefits we experience as a result.

## Details
### Outline
1. A description of our pull request workflow when a change was spread across multiple repositories
1. Pains of that workflow
1. Our experience migrating from many repositories to a single repository, why we did it, and the reasons you might not want to
1. Our new pull request workflow, pros/cons thereof, and how we mitigated certain cons
1. Other tools that aid us in achieving a smoother workflow, i.e. backward-compatible practices, continuous integration, etc.
### Audience
* Those wondering how to structure their code base
* Those interested in continuous integration
* Those wondering how to preserve commit history through a monorepo transition
### Takeaways
* The pros/cons/use cases for a monorepo over multiple repositories
* Considerations/techniques when moving to a monorepo

## Pitch
Many organizations reach a point where there is debate about storage and structure of their code base.
We present some of the considerations and process around choosing to go the monorepo route
without claiming that it is the appropriate choice for every situation.

Once we decided that a monorepo might be an appropriate solution for our use case,
I led the effort in funneling our existing repositories into a monorepo.

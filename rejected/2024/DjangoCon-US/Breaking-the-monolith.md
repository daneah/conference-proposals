# Breaking the monolith

Proposed jointly with @adandavati

## Abstract

As engineers we make decisions every day that can impact our systems for years to come. What happens when the solutions of yesterday become the problems of the present?

In this talk we explore the drivers, tensions, and methodologies that go into an ever-evolving production code base.

## Description

The debate around monolithic and modular systems drives many teams to rehash old decisions and actions, producing a never-ending cycle of work tangent to what they’re really trying to achieve. Whether your team is currently moving toward a monolith or away from one, it remains critical that the quality of the system and processes around it progress forward lest you continue this vicious spiral.

As our Django systems have evolved over the years, several different factors have influenced our thinking and action:

* Team organization and ownership
* Packaging and deployment infrastructure
* Reuse and recomposition of existing features
* Cognitive load and the blast radius of changes

We attempt to claim not that monoliths or modules are the superior solution, but that with the right tools you can arrive at a solution that works within your organizational constraints. We cover a case study and methodology developed over years of practical production experience.

### Thematic Ideas

- The initial creation of our monorepo solved numerous problems, but created problems that would take 1-2 years to fully present.
- The way we worked together and the size of our teams resulted in different architecture needs for our monorepo.
- Methodology may be the same and could be right or wrong depending on the way we work and the org.
- We had a problem, we solved it. Then we had a better problem that we solved by reverting our solution, without getting the first problem back. We outgrew our initial solution and problem to a degree.

## Outline

- Creation of the monorepo
  - Initial excitement and convenience we experienced
  - The reasons behind why we felt we needed it
    - basically one big team working on things, easy to do cross-work
    - lack of a packaging artifact repository, and installing from Github was a bit whack
    - Local development and the need to regularly modify many apps
- The process of dissolving the monorepo
- Attempts made along the way to decouple ourselves
  - Reliance on packages and artifactory
- The size of our team and our team structure during this process
- Micro frontends further decoupling our apps, allowing us to update something in many places without many deploys
- Tools/processes that helped along the way
  - Backstage
    - Templates
    - Soundcheck

# graphene-django or: How I learned to stop RESTing and Love the Graph

## Pitch

django-rest-framework is the tried and true approach for Djangonauts building RESTful APIs. In the era of the JAMstack and the advent of typed, composable queries, what story does Django have to tell about GraphQL?

In this talk you'll learn about Django-Graphene and hopefully come to love it.

## Description

Though controversial, people generally agree that a major value of Python type hints is safety. Robust type safety reduces a whole category of defect to nothing, allowing developers to focus on bigger problems. What if we could do this for our API calls?

GraphQL provides not just a query language, but a type system. The producer and consumer are both aware of the type schema, enabling a boost in productivity at an integration point where mistakes commonly occur. Django has long been a full stack engine at its core, and then a RESTful API engine with the wide adoption of django-rest framework. Where can it go next?

The graphene-django package enables a Django project to provide a GraphQL endpoint built from its models. Using a declarative style most Djangonauts will find beautifully familiar, graphene-django helps developers spin up APIs quickly for consumption by client-side GraphQL consumers like [Apollo](https://www.apollographql.com/).

If you attend this talk, you'll come away having learned:

* How GraphQL compares to REST
* Why this approach can help you maintain loose coupling between teams
* How to build GraphQL types on top of your Django models
* How to provide a schema that resolves queries to model fields
* How to try your new API out in the browser

## Notes

I've been a full stack web application developer for the last six years, and have most recently been exploring how our organization can migrate from server-rendered Django pages to client-side applications that query Python-based APIs. GraphQL is a major part of this work, and graphene-django helps ensure that those Python APIs can specifically be Django APIs.

# Serverless Django with Zappa

## Abstract

You’ve finally built out a project that you’d like to share with the world.
That’s amazing!
Where do you host the thing?
Enter Zappa.
This framework on top of AWS Lambda will allow you to bring your application to the masses
with a light configuration
and—if you’re lucky—a light bottom line.

## Details

A common set of considerations when planning to release a new application are around hosting and resources:

1. Which platforms will support my app?
1. What OS should I use?
1. What WSGI server should I use?
1. How much memory and CPU do I need?

Zappa, a framework for running serverless WSGI applications on top of AWS Lambda,
can help address these and other questions around application deployment.
With some configuration (as code), Zappa can get you up and running quickly,
letting you focus on developing the application instead of the infrastructure.

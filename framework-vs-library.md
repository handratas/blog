# Framework vs Library

![framework-vs-library-illustration](https://user-images.githubusercontent.com/12756891/118480235-2d3faa80-b73c-11eb-9a82-93d4a5050ff1.png)

## Framework
- When building an application using a particular framework, the application lives inside the framework.
- Although not always been the case, when an application is required to inherit from some framework class, it commonly become noticeable.
- From the viewpoint of the application, the framework is the whole world.
- The framework is the all-powerful environment which can do everything the application would ever want (for some particular domain, at least).

### Benefits of a framework
> Inversion of control is a key part of what makes a framework different to a library. A library is essentially a set functions that you can call, these days usually organized into classes. Each call does some work and returns control to the client.
> A framework embodies some abstract design, with more behavior built in. In order to use it you need to insert your behavior into various places in the framework either by subclassing or by plugging in your own classes. The framework’s code then calls your code at these points. 
> ~ Martin Fowler

### Downsides of a framework


## Library 
- Alternatively, an application can be writing using libraries (and it’s always libraries, plural, it’s never just the one).
- In that design, a library is just tacked on to the side of the application.
- The application stands on its own, it has an identity outside of a particular framework, and it just uses libraries to do some part of the work.

> source : [Tom Lokhorst's blog](http://tom.lokhorst.eu/2010/09/why-libraries-are-better-than-frameworks)

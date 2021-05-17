# Framework vs Library

![framework-vs-library-illustration](https://user-images.githubusercontent.com/12756891/118480235-2d3faa80-b73c-11eb-9a82-93d4a5050ff1.png "Framework vs Library Illustration")

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
- First of all, frameworks require a lot from client code. In some OO frameworks the application is required to implement an interface, or worse, to inherit from a framework baseclass.
- Frameworks are also notoriously hard to replace. Precisely because the framework is the application’s whole world.
If you’re using an encryption library you don’t like, you can replace it by some other one.
In frameworks, this is not the case, you can’t just replace a framework.
The best you can hope for is to just add a new encryption library, bypassing the capabilities build-in to the framework.
Granted, replacing a library might be some work, since the API’s for the different libraries can be quite different, but it’s probably doable.
- The same, hard-to-replace argument can be used against platforms, but there I think it’s less applicable.
An application usually is better, the more native to the platform it feels (and is).
For example, a native OS X application usually works a lot better than something that barely uses OS X’s capabilities.
An application that uses more of a framework doesn’t feel more native, it just feels more default.
- The biggest problem I have with frameworks is the tight coupling between the application and the framework.
The application calls the framework to do certain things, and the framework calls the application back.
This tight coupling goes directly against well known software design principles, and it is the ultimate source of the problems described above.

## Library 
- Alternatively, an application can be writing using libraries (and it’s always libraries, plural, it’s never just the one).
- In that design, a library is just tacked on to the side of the application.
- The application stands on its own, it has an identity outside of a particular framework, and it just uses libraries to do some part of the work.

> source : [Tom Lokhorst's blog](http://tom.lokhorst.eu/2010/09/why-libraries-are-better-than-frameworks)

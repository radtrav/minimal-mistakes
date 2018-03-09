---
title: 'The Two Singleton Pattern Gotchas in Node'
categories:
published: true
---


The singleton pattern is used when we want to ensure that there is only one instantiation of a class. This pattern allows the class to control this sole instantiation.

So how do we create singletons in Node.js? Well, some people will tell you that when you require in a module you are creating a singleton. This is true for most cases but not strictly true. It doesn't matter if you require in the module two time or three times, it will still only exist as a single instance.

So why is this true for most cases but not "strictly true"?

If the module is required in twice, it may create two instances if the modules are cached differently.

So when would they be cached differently? We have two potential reasons why two identical modules may be cached differently:

1. When Node caches a module the case of the filename is IMPORTANT

For example, require(‘./foo’) and require(‘./FOO’) return two different objects, irrespective of whether or not ./foo and ./FOO are the same file


2. Modules are cached based on their resolved filename

Since modules may resolve to a different filename based on the location of the calling module (loading from node_modules folders), it is not a guarantee that require(‘foo’) will always return the exact same object, if it would resolve to different files.


It is important to keep in mind these two gotchas when trying to implement the Singleton Pattern in Node.



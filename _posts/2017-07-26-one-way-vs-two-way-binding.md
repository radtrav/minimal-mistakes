---
title: 'One Way Vs Two Way Binding'
categories:
published: true
---

What is the difference between one way and two way data binding? Often when this question comes up the source is a comparision between Angular(1) and React. It is important to note that Angular 2, being a complete rewrite,  has some important differences compared to Angular 1. Angular 2 still supports two way binding, however it doesn't come baked in like Angular 1.

To understand the differences in bindings we need to understand the differences between Angular 1 and React.

First off Angular is an MVC front end framawork. According to the Gang of Four's "Design Patterns: Elements of Reusable Object-Oriented Software"

> "MVC decouples views and models by establishing a subscribe/ notify protococol".

 This means that the view (the V in MVC), will reflect the model (the M in MVC). Whenever the model's data changes, the model will notify any views that depend on it. This approach lets you attach multiple views to a model to provide different presentations. The controller, the C in MVC allows the decoupling of the model and the view using a subscribe/ notify protocol.

React on the other hand is only a view library. The direction of the data only flows downward from parent components to child components. To get any communication between the application and the view you need to use callbacks. The problem with this is that it can get complicated writing your own callbacks that get fired on UI interactions.

 Angular(1) has less boilerplate than React because you already get 2 way data binding. In React, to get anything approaching 2 way data binding you need to write your own callbacks. This can lead to more code, however if you wrote it, you should understand the data flow better. Angular's 'magical 2 way data binding' may lead to gaps in knowledge about your application's data channels and therefore bugs down the line.

The benefit of one way data binding is that data only flows in one direction, so it is easy to track down what caused change.




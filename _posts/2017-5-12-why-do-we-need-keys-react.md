---
title: 'Why Do Arrays of React Elements Need Keys?'
categories:
published: true
---
![alt text](http://www.hackingwithreact.com/read/img/missing_key.png)

http://www.hackingwithreact.com/read/img/missing_key.png

We've all see this error before in React. Its a very easy fix, but what is actually the significance of keys?

Keys ensure identity and allow React to distinguish between elements and to decide what needs to be rendered or re-rendered.

Elements with keys will be reordered instead of destroyed.

Not everything in the DOM has a representation in the Virtual Dom. Not having keys will lead to recreating DOM nodes instead or reusing a DOM node to render another component and therefore losing untracked state.

This can have performance implications, depending on the key you choose you may be avoiding wasterful re-renders.
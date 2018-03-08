---
title: 'CSS Reset vs Normalize.css'
categories:
published: true
---

![alt text](https://assets.hongkiat.com/uploads/thumbs/640x410/normalized-css-twitter.jpg)


What is the difference and why should I care?

### Css Reset

 The browser by default adds certain styles to elements such as padding and margins. resetting removes browser styling so that you can start with essentially a blank canvas. The problem with resets are the you will lose some useful styles that you gain with the browser.

### Normalize.css:

 Normalize.css ensures that all html elements render the same way consistently in all
 browsers. Normalize.css won't reset every  browser defined style, it will preserve useful browser defaults like font styles, margins and line height. It will correct bugs and common browser inconsistencies that are out of the scope of resets.

### My Preference

I lean towards Normalize.css because it is based on a lot of cross-browser research and testing. I am all for standing on the shoulder of giants rather than re inventing the wheel. Even if you are not adding Normalize.css directly, large projects like Twitter Bootstrap and HTML5 Boilerplate are already using it. Alot of smart people have come together to develop a solution for cross-browser incompatibilities so why not take advantage?
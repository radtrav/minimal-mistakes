---
title: 'The Wrapper Div is Dead! - Well Sorta'
categories:
published: true
---
![alt text](https://cdn-images-1.medium.com/max/1200/1*Wm93IONcgMK6eaQkbGaz1Q@2x.png)

There is one feature that I am pretty excited about in React 16. You can now render an array of elements instead of enclosing everything in a wrapper div. You can also now return a string directly without wrapping it in a div or span. This is great as it reduces clutter. The one gotcha is that on each component in the array you need to specify a key.  I have noticed using the Chrome React Dev Tools, that sometimes it can be painful to find the right component due to such deep nesting. Doing away with superfluous divs should make markup much cleaner and easier to wade through. Here are a couple examples below.


```javascript
render() {
  return [
    <li key="1">Hey Mom</li>,
    <li key="2">Look</li>,
    <li key="3">No Hands!</li>,
  ];
}
```

```javascript
render() {
  return 'Look! no span no div but still chilling!';
}
```

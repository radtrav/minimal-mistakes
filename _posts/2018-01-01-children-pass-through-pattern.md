---
title: 'The React Children Pass-Through Pattern'
categories:
published: true
---
![alt text](http://cdn.newsapi.com.au/image/v1/9b40c7068b9f6a4e999fc4a77c014156)


## The Children pass-through pattern.

Say for example we have a component that simply applies some context to its children. Perhaps this is the only purpose of this component. What is the best way to return the component's children inside of the render function?

We have two options.

```javascript

// option 1: wrap the children in an extraneous div
return <div>{this.props.children}</div>

// option 2: unhelpful errors
return this.props.children;
```

it turns out React has a solution as part of it's Children API

```javascript
return React.Children.only(this.props.children);
```

This method verifies that children has only one child (a React element) and returns it. Otherwise this method throws an error.

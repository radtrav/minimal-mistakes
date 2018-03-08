---
title: 'create-react-app vs react-slingshot'
categories:
published: true
---



## I love create-react-app but I don’t regret using react-slingshot

![alt text](https://cdn.dribbble.com/users/464284/screenshots/3354218/react-slingshot-hires_1x.jpg)

We initially started our project using the React-Redux starter kit react-slingshot put together by Cory House. This starter kit is great because it includes a lot of things that you would expect in a good boilerplate: testing, linting , hot reloading etc. The best part is that he has an excellent course on Pluralsight that covers alot of the configuration; from the npm scripts to babel, to web pack. Honestly the trickiest part about starting a new project is often deciding on the ideal configuration.

Using a boilerplate like this really lightened the load. However, that being said as we start using this we noticed there were some things that were lacking. This boilerplate uses react-routerV3 instead of V4, something that is excusable given that at the time of picking up this boilerplate V4 was just coming out. We found that sometimes we wanted use the latest features that were included in create-react-app like using Flow Types and the newest Es7 features. Of course some of these were easily fixable by just configuring things ourselves. We started to notice that a lot of the community had started to use create-react-app and so a lot of the features that were included in create-react-app became somewhat standard. Now that we are migrating parts of our application over to admin-on-rest and using create-react-app i can appreciate all the abstraction that create-react-app does for you.


However I do not regret starting with react-slingshot because it really helped me understand the inner plumbing of a well configured application. Having to add on “pipes” to the plumbing system by hand really helped me understand the React Ecosystem. I would advise those interested in learning the inner workings to eject and try and figure out what create-react-app is doing for you behind the scenes.
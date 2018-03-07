---
title: 'Experimenting With The Admin-On-Rest React-based Framework'
categories:
published: true
---

I came across admin-on-rest the other day and was intrigued with the some of the built in features that it comes with. Admin on rest is developed by marmelab and has 3000 stars on GitHub. It has about 100 contributors and  has a lot of recent activity. Admin-on-rest basically acts as an adaptable admin panel for any rest backend.

They are self described as: "A frontend Framework for building admin applications running in the browser on top of REST services, using ES6, React and Material Design."It helps create a front end with features resembling many database clients. The ability to Create, Read, Update and Delete database entries from the front end.

Admin-on-rest uses a function called the REST client which translates REST calls to HTTP requests. It abstracts away a lot of the logic and cuts down on tedious boilerplate. Writing a REST client is quite simple and saves a lot of legwork in the long run.

Currently the 55Circles app is coming along nicely, however some of the CRUD features have not been fully implemented yet. We are currently in the stage of seeing whether using the admin-on-rest framework for some parts is worth it. Our application requires a lot of CRUD work which is handled beautifully with AOR. We are hoping that AOR will reduce some of the time that it would take to implement internationalization, authorization of view - something we will need once we implement different member tiers (admin, paid, free etc).
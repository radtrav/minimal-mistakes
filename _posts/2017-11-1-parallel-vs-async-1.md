---
title: 'Understanding Parallel vs Asynchronous Programming'
categories:
published: true
---
![alt text](https://d2uetvsama7sl8.cloudfront.net/prod/wp-content/uploads/2016/03/17131608/async.png)

## Understanding Parallel vs Async

I think before I go into what parallel and async is I should cover what non parallel programming is. Non parallel code is code that is typically easy to reason about. It is intuitive top down left to right code. Task a executes and once that has finished task b executes and then after that task c etc.

So what is parallel programming ? Parallel programming means  processing can be done simultaneously via different threads. These days most computers have four core CPUs , meaning one process can run on each core. If you are trying to make cars using parallel programming that would be like making four cars at once. However there are instances when things cannot be run in parallel, for example if one process is dependant on another one finishing.

Parallel programming is useful when performance is critical. Applications working with big data like Hadoop are excellent use cases. In most cases using parallel programming for web apps would be overkill and extremely expensive to architecture.

Parallel programming is still in its early stages (it has only existed for the last 20 years), given that multiple cores in cheap computers are relatively new. Most programming languages were not designed with parallel processing in mind.

Asynchronous code is run on  a single thread and not on multiple cores. Asynchronous code is non blocking which means when a long running task such as network requests or disk I/O is needed, the request begins without blocking for the response. Once the response is ready, an interrupt is  fired which causes an event handler to run. UI interfaces are naturally async, the event loop is interrupted once a user triggers and event handler.
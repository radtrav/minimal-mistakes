---
title: 'React 16 Error Boundaries'
categories:
published: true
---

![alt text](https://cdn-images-1.medium.com/max/1200/1*Wm93IONcgMK6eaQkbGaz1Q@2x.png)

Previously when runtime errors occurred during rendering the whole app was unmounted to prevent the display of corrupted data. React 16 implements a new strategy of error handling called error boundaries, which are special types of components. Instead of crippling the application whenever an error occurs a fall back UI is showed. It can be thought of as analogous to try-catch statements. I look forward to experimenting with these in the future.
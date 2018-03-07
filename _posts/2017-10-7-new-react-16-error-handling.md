---
title: 'React 16 Error Boundaries'
categories:
published: true
---

Previously when runtime errors occurred during rendering the whole app was unmounted to prevent the display of corrupted data. React 16 implements a new strategy of error handling called error boundaries, which are special types of components. Instead of crippling the application whenever an error occurs a fall back UI is showed. It can be thought of as analogous to try-catch statements. I look forward to experimenting with these in the future.
---
title: 'What Makes the Virtual DOM so Fast?'
categories:
published: true
---

How does the virtual DOM work?

1. Whenever any underlying data changes, the entire UI is re-rendered as Virtual DOM representation.

2. The difference between the previous DOM representation is calculated

3. The real DOM will then update with only the differences.

Because the real DOM only updates based on the differences there are fewer updates which results in a faster UI.


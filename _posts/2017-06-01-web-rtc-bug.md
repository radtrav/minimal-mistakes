---
title: 'The Chrome WebRTC Bug'
categories:
published: true
---

![alt text](https://webrtc.org/assets/images/webrtc-logo-horiz-retro-750x140.png)

We decided to move away from building our own in-browser WebRTC solution for our video conferencing features.

 We feel somewhat that our hand has been forced given the chrome WebRTC audio in bug which seems to affect MacOS users. What happens is that when a connection is made if the browser has been left open for a while audio might not be sent out. The only solution at this time is to restart chrome, which is not convenient for our users. This is something that you may have noticed before using video conferencing apps on Chrome, like Google Hangouts or Facebook Messenger Video.

  This problem doesn’t seem present in Firefox, and it seems to be something that has plagued google for a while, since 2012 infact! They have announced that it is their utmost priority to fix this issue.

  At first naturally we assumed that the bug existed in our own code, we reached out to Tokbox for assistance after days of searching for an answer with little results. Tokbox were the ones that informed us that the bug was not on their side either but inherent to Chrome.
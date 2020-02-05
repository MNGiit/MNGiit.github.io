---
layout: post
title:      "JavaScript Event Handling"
date:       2020-02-05 04:58:41 +0000
permalink:  javascript_event_handling
---


Usually the user does something to a web browser, and thanks to JavaScript, the developer can listen to the user's action and do something about it. JavaScript can recognize certain things that happens inside a browser, which we'll call Event Listening, and can do something when it listens to a specific action, which we'll call Event Handling.

Some types of events that JavaScript can listen to are:
* Mouse over (moving the mouse over something like an image)
* Mouse clicking
* Key pressing
* Browser manipulation (resizing the browser)
* On load (the web page loaded)
* etc

Notice it's not just from the user doing something directly. It can be something like the web page loading.

To listen to, or hear an event and start executing a callback function to do something after listening, we can use addEventListener(). The syntax looks like this:
`element.addEventListener(event, function, useCapture)`
useCapture is optional so doing something like this will work too:
```
element.addEventListener(event, function)
```

For more information about it, visit [here](https://www.w3schools.com/js/js_events.asp).



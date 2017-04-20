# Laziness.js
A collection of functions to be used if you're a lazy sod like me. These typically go into each project I write in Node to make life easier, and save *literally* 3 seconds of my time.

# Contributing

Got any lazy JS code that might be useful to other people? Fork and update the README with your code and send a PR. Don't be *too* lazy and add in some documentation (even a single comment) and a header so we know what the hell's going on.

# Auto launching your browser.

```
var child = require('child_process').exec;

//Place after all of your code in server.js/app.js whatever.

(function init() {
  (function launchBrowser() {
    child('start chrome http://localhost:' + YOUR_PORT);
  })();
})();
```

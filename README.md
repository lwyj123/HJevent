# HJevent
a wheel of EventEmitter use es6 (HJproject)

# Install

```javascript
<script src="HJevent.js"></script>
```

# Usage
### HJevent.on(event, listener)

`event` a string of your event.

`listener` a callback function run when emited.

### HJevent.off(event, listener)

`event` a string of your event.

`listener` the callback function you wanna unbind.


Example

```js
var eventEmitter = new HJevent();
var echotest = function() {
    alert("this is a test");
});


eventEmitter.on("echotest", echotest);

eventEmitter.emit("echotest");

eventEmitter.off("echotest", echotest);

eventEmitter.emit("echotest");
```

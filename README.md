# post2ws

Runs an http server on :5000 that you can POST to. Every POST is broadcast on a websocket your client can connect to.

To post, `curl localhost:5000 -d'what ho!'`. 

To connect to the websocket, in javscript

```
var ws = new WebSocket("ws://localhost:5000")
ws.onmessage = function(msg){console.log(msg)}
```


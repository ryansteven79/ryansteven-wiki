<!-- TITLE: node.js Server With Express -->


```javascript
var express = require("express");

var app = express();

var PORT = process.env.PORT || 8080;

// Routes
app.get("/file-path", function(req, res) {
  res.render("index");
});

app.listen(PORT, function() {
  // Log (server-side) when our server has started
  console.log("Server listening on: http://localhost:" + PORT);
});
```

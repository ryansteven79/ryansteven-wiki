<!-- TITLE: node.js Server With Express -->


```javascript
var express = require("express");
var exphbs = require("express-handlebars");

var app = express();

var PORT = process.env.PORT || 8080;

app.engine("handlebars", exphbs({ defaultLayout: "main" }));
app.set("view engine", "handlebars");

// Routes
app.get("/file-path", function(req, res) {
  res.render("index");
});

app.listen(PORT, function() {
  // Log (server-side) when our server has started
  console.log("Server listening on: http://localhost:" + PORT);
});
```

FriendFinder
- .gitignore
- app
				- data
						- friends.js
				- public
						- home.html
						- survey.html
				- routing
						- apiRoutes.js
						- htmlRoutes.js
				- node_modules
				- package.json
				- server.js


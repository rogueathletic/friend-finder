
<div align="center">
  <span> <a href="#top"> Home </a> </span> | 
  <span> <a href="#intro"> D E M O </a> </span> | 
  <span> <a href="#htss"> H T M L \ C S S </a> </span> | 
  <span> <a href="#express"> E X P R E S S </a> </span> | 
  <span> <a href="#heroku"> H E R O K U </a> </span> | 
  <span> <a href="mailto:jason@rogueathletic.com" target="_blank"> Contact </a> </span>
</div>









<details style="-webkit-appearance: none;" align="center"><summary align="justify"><h1>Best Friend Finder</h1></summary>
  <span><h2>UCSD</h2></span><span><h3>Full Stack Web Dev Assignment 14</h3></span>








<details align="center"><summary align="justify"> D E M O </summary><a href="https://www.youtube.com/watch?v=JHurCXqH6KI">
<img src="https://i.imgur.com/cS1UuUW.png" width="80%">
</a></details>

<details align="center"><summary align="justify"> S E R V E R . J S </summary><p>The server configuration</p> 
  ```js
  //
  // Pull in required dependencies
var express = require('express');
var bodyParser = require('body-parser');
var path = require('path');

// Configure the Express application
var app = express();
var PORT = process.env.PORT || 8080;

// Expose the public directory to access CSS files
app.use(express.static(path.join(__dirname, './app/public')));

// Add middleware for parsing incoming request bodies
app.use(bodyParser.json());
app.use(bodyParser.urlencoded({ extended: true }));
app.use(bodyParser.text());

// Add the application routes
require(path.join(__dirname, './app/routing/apiRoutes'))(app);
require(path.join(__dirname, './app/routing/htmlRoutes'))(app);

// Start listening on PORT
app.listen(PORT, function() {
  console.log('Friend Finder app is listening on PORT: ' + PORT);
});
```
</details>

<details align="center"><summary align="justify"> E X P R E S S . J S </summary>content</details>

<details align="center"><summary align="justify"> H E R O K U </summary>content</details>

<details align="center"><summary align="justify"> C O N T A C T </summary>  <span> <a href="mailto:jason@rogueathletic.com" target="_blank"> Contact </a> </span></details>
</details>


<details><summary>
# friend-finder</summary>
Best friend finder app utilizing API, MYSQL, Jquery, HTML, CSS, Javascript, Heroku, Github and more...
</details>

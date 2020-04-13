# Introduction
Express is a minimal and flexible Node.js web application framework that provides a robust set of features for web and mobile applications. </br>
It is:</br> - Highly extensible </br>
       - Highly flexible

# Installing Express.js
In the terminal of the root project directory: ```npm install --save express```

## Importing it
At the top of your file: ```const express = require('express')```

## To use it
```const app = express()```` //This is creates an express application ```

## Creating a server using Express
```
app.listen(3000)
```

# Middleware
Middleware literally means anything you put in the middle of one layer of the software and another. Express middleware are functions that execute during the lifecycle of a request to the Express server. Each middleware has access to the HTTP request and response for each route (or path) it's attached to.

## Adding Middleware
```
app.use((req, res, next) => {
next(); // To call the next middleware
}
```
## Sending Responses with express.js
```res.send()```

## Parsing Incoming Requests
### Install a 3rd Party application 
```npm install --save body-parser```

### Import it
```const bodyParser = require('body-parser')```

### Use it
``` app.use(bodyParser.urlencoded({extended: true}))```

## Limiting Middleware execution 

**app.use** executes for both POST and GET requests

### To filter for post requests: 
```
app.post()
```
### To filter for get requests: 
```
app.post()
```

# Food-order-system

## Back End Start

### Install nodejs packes
- npm init //Create package       
- npm i express  
- npm i body-parser //Input get from
- npm i nodemon  // Node server
- npm i mongodb  //MongoDb
- npm i password-hash  //Password Hash
- npm i passport //authentication
- npm i flash
- npm i path
- npm i cookie-Parser
- npm i morgan
- npm i connect-flash
- npm i express-session
- npm i multer

### Include packes
- var express = require('express');
- var app = express();
- var port = process.env.PORT || 2223;
- var mongoose = require('mongoose');
- var passport = require('passport');
- var flash = require('connect-flash');
- var path = require('path');
- var morgan = require('morgan');
- var cookieParser = require('cookie-parser');
- var bodyParser = require('body-parser');
- var session = require('express-session');
- var multer = require('multer');


### Add CSS/JS later using EJS with nodejs/express
- server.js file add app.use(express.static(__dirname + '/file name'));
- Index.ejs file need to add <script src="/javascripts/jquery.js"></script>    

## Directory access
- app.use(express.static(__dirname + '/authentication/front_end')); //Access javascript file
- app.use(express.static(__dirname + '/admin_panel')); 
- app.use(express.static(__dirname + '/user_panel'));
- app.use(express.static(__dirname + '/home')); 
- app.use(express.static(__dirname + '/uploads')); 
- app.use(express.static(__dirname + '/authentication'))
- app.set('views', path.join(__dirname, 'views'));

### Collections
- var Detail = require('./authentication/app/models/foodDB'); //FoodInfo
- var __User = require('./authentication/app/models/userDB'); //CustomerInfo
- var __Admin = require('./authentication/app/models/adminDB'); //AdminInfo

// Our Database
var configDB = require('./authentication/config/database.js');


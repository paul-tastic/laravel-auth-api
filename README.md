## Overview

This project is designed to be a template for PHP/Laravel backend with restful-API endpoints that will support both a generic 'product' CRUD operation but also authentication passed through Laravel's Sanctum all up against a sqlite database. It is re-useable across a couple different projects I am working on that need to access a database as authenticated users (with a mobile device front-end).  

Once authenticated and logged in, user is given a token. That token will be stored in the device storage and used during all subsequent calls for data.  

The database type can be any mainstream type, but I used sqlite in this instance because the local development tools I have allow for quick and no-fuss implementation for develoment purposes. It is easily configured for any database and location though.  

## Public endpoints:

/register -> "register" method  
/login -> "login" method  
/logout" -> "logout" method  

## Protected endpoints (must be authenticated with token)

/products -> "index" method (show all product offerings)  
/products/{id} -> "show" method (show specific product offering)  
/products/search/{name} -> "search" method  
/products -> "store" method (add a product)  
/products/{id} -> "update" method (modify a product's details)  
/products/{id} -> "destroy" method (delete a product)  

## to run this locally:

clone github repo to local machine  
php artisan serve  
php artisan migrate  
you can use postman/insomnia to hit the endpoints (http://localhost:8000/api/...)  
you can use DB Browser to view database changes  

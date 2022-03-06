## Overview

This project is designed to be a PHP/Laravel backend with restful-API endpoints that will support both a generic 'product' CRUD operation but also authentication passed through Laravel's Sanctum all up against a sqlite database. It's a template for future projects.

The use of sqlite is to save time on the initial development of the template due to the ease of php artisan in laravel and sqlite db tool... but will be converted to Mysql for production once the architecture is built out.

to run this and test it out:
clone github repo to local machine
php artisan serve
php artisan migrate
you can use postman/insomnia to hit the endpoints
you can use DB Browser to view database changes

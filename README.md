# eStore
COSC 631 - eCommerce &amp; Web DB Infrastructure
step 1 Download Composer from https://getcomposer.org/download/
step 2 Select C:/XAMPP/Php/php.exe
step 3 PowerShell cd C:/XAMPP/htdocs> composer create-project --prefer-dist laravel/laravel COSC631_laravel 
step 5 C:/XAMPP/htdocs> cd COSC631_laravel 
step 6 C:/XAMPP/htdocs/COSC631_laravel> php artisan serve
Laravel development server started: http://127.0.0.1:8000
C:/XAMPP/htdocs/COSC631_laravel> cd resources/views
open welcome.blade.php
change "Laravel" to "Welcome to COSC631 Project"

open .env
change database name to eStore

DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=eStore
DB_USERNAME=root
DB_PASSWORD=

step 7 C:/XAMPP/htdocs/COSC631_laravel>php artisan migrate

view in phpMyAdmin

http://127.0.0.1:8000/hello
C:/XAMPP/htdocs/COSC631_laravel/route/view/web.php

Route::get('/', function () {
    return view('welcome');
});
Route::get('/hello', function () {
    return '<h>hello world</h>';
});

http://localhost:81/phpmyadmin/

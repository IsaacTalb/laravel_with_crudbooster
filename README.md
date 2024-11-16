## Welcome To CRUDBooster
CRUDBooster is CRUD Generator for laravel, with the most important features web application development. It's easy, flexible, and powerful.

## Laravel 6.* / 7.* /

Installation
Please make sure you have install laravel project, please follow https://laravel.com/docs/7.x/installation

you can use this command for creating laravel project
## composer create-project laravel/laravel your-project-name


Open the terminal, navigate to your laravel project directory. You can use by this command:
## cd your-project-name

and then in terminal run this:
## composer require crocodicstudio/crudbooster=5.6.

and you will be prompted as error that you need something CBseeder or seeders: 

Setting the database configuration, open .env file at project root directory
DB_DATABASE=**your_db_name**
DB_USERNAME=**root**  (change as you need)

Run the following command at the terminal
## php artisan crudbooster:install

Ensure the CBSeeder file exists in the database/seeds directory (for older Laravel versions) or database/seeders (for Laravel 8 and above). If not, create it:

## php artisan make:seeder CBSeeder

and after that; you need run this;
## php artisan db:seed

Backend URL
/admin/login

default email : admin@crudbooster.com
default password : 123456


Debugging Issues
If the issue persists:

Check Laravel version compatibility: Ensure CRUDbooster supports your Laravel version.
Clear cache and autoload: Run the following commands to clear caches and reload class maps:

### php artisan config:clear
### php artisan cache:clear
### php artisan route:clear
### composer dump-autoload


let me know if you have any problems
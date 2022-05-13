# interview-laravel-9
Gamers Hunter interview repository, uses Laravel 9.12.2

## Project setup
This guide assumes you already have Git, PHP8, composer, NodeJS and MySql installed, and have cloned the repository. 

1. Duplicate .env.example file to .env and update database connection values to your corresponding database and schema values.
2. Run `composer install` to install dependencies
3. Run `php artisan key:generate` to generate a unique app key
4. Run `php artisan migrate` to run database migrations
5. Run `php artisan db:seed` to run seeders
6. Run `npm install && npm run dev` to compile assets
7. Run `php artisan serve` to start serving your application
8. Access app on `http://localhost:8000` on your browser

## Project update
- Run `composer install` to update dependencies
- Run `php artisan migrate` to run missing database migrations

## Debugging with VS Code
1. Download and [install xDebug](https://xdebug.org/docs/install)
2. Install the PHP Debug by xDebug extension for VS Code
3. Open your php.ini file and add the following to enable debugging
```
xdebug.mode = debug
xdebug.start_with_request = yes
xdebug.client_port = 9003
```
4. Open `web.php` or any php file so VS code recognizes php project
5. Go to the `Run` menu and `add configuration`, select `xDebug` if prompted, make sure to set port to the one you chose.

You should now be able to debug and use breakpoints inside VSCode. 

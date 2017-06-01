# laravel-start

Some simple tips to start with laravel

### PHP STORM ###

Install plugin : Laravel plugin
Install Theme : Material Theme UI

### Install Laravel ###

composer create-project laravel/laravel

## AUTH ##

php artisan make:auth

### To delete use of Route /register from Auth ###

In file RegisterController add those functions : 

public function showRegistrationForm() {
   return redirect('login');
}
public function register () {}

### SQL Error with migration on Laravel 5.4 ###

Set this line of code in file AppServiceProvider (in function boot()) :

Schema::defaultStringLength(191);

## INTERESTING PACKAGE ##

Gestion formulaire : https://laravelcollective.com/docs/5.2/html
Debugbar : https://github.com/barryvdh/laravel-debugbar

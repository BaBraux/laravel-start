# laravel-start

Some simple tips to start with laravel

### PHP STORM ###

Install plugin : Laravel plugin
Install Theme : Material Theme UI

#Install Laravel

composer create-project laravel/laravel

#Use Authenticate

php artisan make:auth

#SQL Error with migration on Laravel 5.4

Set this line of code in file AppServiceProvider (in function boot()) :

Schema::defaultStringLength(191);

#To delete use of Route /register from Auth

In file RegisterController add those functions : 

public function showRegistrationForm() {
   return redirect('login');
}

public function register () {}

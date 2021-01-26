# laravel-bootstrap
Laravel with bootstrap - sample app in lessthan 10 mins

Here I given very simple instructions as per the laravel docs 

Open CLI/Command Line Interface

You may install the Laravel Installer as a global Composer dependency, run the following command:
composer global require laravel/installer

Create Laravel App:
laravel new example-app

Go to the App:
cd example-app

Run App to test:
php artisan serve

Open the App in browser using below url:
http://127.0.0.1:8000/

If all good and you can see laravel welcome page
Note: it will not show you Login / Register links, they will show up once completing the following steps.

Come to CLI/Command terminal exit from the app.

We simply need to install the laravel/ui package using Composer and installing the Bootstrap 4 package from npm.
The laravel/ui package provides the scaffoldings for bootstrap, vue and react. And the auth scaffold for login and registration.

Head over to your terminal, navigate to your app folder and run the following command:
composer require laravel/ui

After successfully installing the package, we install Bootstrap 4 in our application using the following command:
php artisan ui bootstrap

You can also install the auth scaffoldings using the following command instead:
php artisan ui bootstrap --auth

Finally, you need to install the bootstrap package and the related frontend dependencies such as jquery from npm using the following command:
npm install

npm run dev

If you see message "Complied successfully" 
- /js/app.js 
- css/app.css
then its all good, otherwise just check the instructions on the command screen and run those commands.

Create mysql database and update .env file with database name

Run the command to update database with tables:
php artisan migrate

Run the app:
php artisan serve

Open the App in browser using below url:
http://127.0.0.1:8000/

Now, you can see the login and registration links.
From here, you can customize the app as per your design requirements.


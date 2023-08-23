# php-study
Study PHP language

## Install PHP for Laravel project
```
sudo apt install php
sudo apt install composer
sudo apt install php-xml
sudo apt install php-curl
sudo apt install php-mysql
sudo apt install php-mbstring
composer create-project laravel/laravel bboard "9.1.*"
cd bboard
composer require laravel/ui
php artisan serve

php artisan make:controller BbsController
```
### If project exist
after install
```
composer install
cp .env.example .env
php artisan key:generate
php artisan config:cache
php artisan serve
```

### Migrations
```
sudo apt install php-sqlite3
php artisan make:migration create_bbs_table --create=bbs
php artisan migrate
```


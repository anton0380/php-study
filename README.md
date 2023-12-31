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
sudo apt-get install libapache2-mod-php php-common php-gd php-intl php-xsl php-zip php-bcmath php-soap php-xdebug php-imagick
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

### Models
```
php artisan make:model Bb
```

### Console
```
php artisan tinker
```

### Rollback
Rollback last migration
```
php artisan migrate:rollback --step=1
```

### Auth
```
php artisan ui:auth
```

### Routes
```
php artisan route:list
```

### Policy
```
php artisan make:policy BbPolicy
```

### Localization
```
composer require arcanedev/laravel-lang --dev
composer require laravel-lang/lang:^10.4.2 --dev
php artisan trans:publish ru --json
```
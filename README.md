# Laravel 8 JWT API 
Based on Laravel 8 JWT

## Source
* https://www.positronx.io/laravel-jwt-authentication-tutorial-user-login-signup-api/

## Installation Guide
    1)Clone Or Download The Repository

    2)Set the .env File with the relevant configuration

    2)Goto to project root and open a Terminal Enter Following Commands 
        * composer install
        * php artisan key:generate
        * php artisan jwt:secret
        * php artisan migrate
        
        
## Errors
    1) Deprecation Notice: Class App\Http\Controllers\API\PassportAuthController located in D:/dev/l8-api/app\Http\Controllers\Api\PassportAuthController.php does not comply with  psr-4 autoloading standard. It will not autoload anymore in Composer v2.0. in phar://C:/ProgramData/ComposerSetup/bin/composer.phar/src/Composer/Autoload/ClassMapGenerator.php:201
    2) Deprecation Notice: Class AWT\Http\Exceptions\InvalidApiLogDriverException located in D:/dev/l8-api/vendor/awt/apilogger/src\Exceptions\InvalidApiLogDriverException.php does not comply with psr-4 autoloading standard. It will not autoload anymore in Composer v2.0. in phar://C:/ProgramData/ComposerSetup/bin/composer.phar/src/Composer/Autoload/ClassMapGenerator.php:201
    3) Solution 
        * "namespace App\Http\Controllers\API;" -> "namespace App\Http\Controllers\Api;"
        * "namespace AWT\Http\Exceptions;" -> "namespace Awt\Http\Exceptions;"
        * composer dump-autoload

## Database conn str
* config/database.php
## Token
* app/Providers/AuthServiceProvider.php

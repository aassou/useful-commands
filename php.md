# PHP Packges and extensions
sudo apt install php7.4-gd
sudo apt install php7.4-xml
sudo apt install php7.4-mbstring

# Symfony commands

php bin/console make:entity

php bin/console make:migration

php bin/console doctrine:migrations:migrate

php bin/console doctrine:fixtures:load --append

# Useful packages

composer require liip/imagine-bundle
composer require symfony/uid
composer require api
composer require monolog
composer require --dev easycorp/easy-log-handler
[
    configuration of easy-log-handler:
    
]
composer require maker
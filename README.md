# cuca
## instalation
curl -s http://getcomposer.org/installer | php
mv composer.phar /usr/local/bin/composer

composer global require "fxp/composer-asset-plugin:1.0.0"
composer create-project --prefer-dist yiisoft/yii2-app-advanced yii-application

sudo apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv 7F0CEB10
echo "deb http://repo.mongodb.org/apt/ubuntu "$(lsb_release -sc)"/mongodb-org/3.0 multiverse" | sudo tee /etc/apt/sources.list.d/mongodb-org-3.0.list

sudo apt-get update

package dependency
packages = [
    "php5-cli",
    "php5-fpm",
    "php5-intl",
    "php5-gd",
    "php5-mysqlnd",
    "php5-curl",
    "php5-mcrypt",
    "php5-xdebug",
    "nginx",
    "mysql-server",
    "git",
    "php5-json",
    "php5-dev",
    "php5-common",
    "php-pear",
    "php-apc",
    "mongodb-org"
]

sudo apt-get install php5-cli php5-fpm php5-gd php5-intl php5-mysqlnd php5-curl php5-mcrypt php5-xdebug php5-json nginx mysql-server git php5-dev php5-common php-pear php-apc mongodb-org

set domain in /etc/hosts

copy nginx.conf to vagrant /etc/nginx/sites-enabled/default

run init to set app environment
./init
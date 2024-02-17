# PHP development setup on Ubuntu machine

## Install Apache

```sudo apt update```

```sudo apt install apache2```

## Install PHP
```sudo apt-get install ca-certificates apt-transport-https software-properties-common wget curl lsb-release -y```

https://launchpad.net/~ondrej/+archive/ubuntu/php/

```sudo add-apt-repository ppa:ondrej/php```

```sudo apt update```

### PHP 7.4 with common extensions
```sudo apt install php7.4 php7.4-cli php7.4-fpm php7.4-bcmath php7.4-curl php7.4-gd php7.4-intl php7.4-mbstring php7.4-mysql php7.4-opcache php7.4-sqlite3 php7.4-xml php7.4-zip libapache2-mod-php7.4 php7.4-common```

### PHP 8.1 with common extensions
```sudo apt install php8.1 php8.1-cli php8.1-fpm php8.1-bcmath php8.1-curl php8.1-gd php8.1-intl php8.1-mbstring php8.1-mysql php8.1-opcache php8.1-sqlite3 php8.1-xml php8.1-zip libapache2-mod-php8.1 php8.1-common```

### PHP 8.2 with common extensions
```sudo apt install php8.2 php8.2-cli php8.2-fpm php8.2-bcmath php8.2-curl php8.2-gd php8.2-intl php8.2-mbstring php8.2-mysql php8.2-opcache php8.2-sqlite3 php8.2-xml php8.2-zip libapache2-mod-php8.2 php8.2-common```

### PHP 8.3 with common extensions
```sudo apt install php8.3 php8.3-cli php8.3-fpm php8.3-bcmath php8.3-curl php8.3-gd php8.3-intl php8.3-mbstring php8.3-mysql php8.3-opcache php8.3-sqlite3 php8.3-xml php8.3-zip libapache2-mod-php8.3 php8.3-common```

For quickly toggling between versions of PHP, I have written a small bash script that can be helpful https://github.com/devfaysal/switch-php-version

## Install Composer
https://getcomposer.org/download/

## Install MySQL
```sudo apt install mysql-server```

https://www.digitalocean.com/community/tutorials/how-to-install-mysql-on-ubuntu-22-04

## Permissions
```sudo a2enmod rewrite```

```sudo chown {your ubuntu username} /var/www```

## Install Git
```sudo apt install git```

## Setup Virtual host
For the Laravel applications I have written a small bash script that can help create a whole Virtual host setup quickly https://github.com/devfaysal/laravel-vhost 

## Install Nodejs
https://stackoverflow.com/a/66166866/6150983
Download LTS version from https://nodejs.org/en (a file like node-v20.10.0-linux-x64.tar.xz will be downloaded)

```sudo apt update```

```sudo apt install xz-utils```

cd into the directory where the file node-v20.10.0-linux-x64.tar.xz downloaded

```sudo tar -xvf node-v20.10.0-linux-x64.tar.xz```

```sudo cp -r node-v20.10.0-linux-x64/{bin,include,lib,share} /usr/```

Check the version to confirm the installation 

```node --version```
```npm -v```








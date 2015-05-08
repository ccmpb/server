# Vagrant & Ansible Webserver 

#### Vagrant config with Ansible provisioning for a LNMP server
#### Included Packages
- php5
- php5-mcrypt
- php-fpm
- mariadb
- nginx

#### How to use
##### VIA Composer
- Add the repo to your composer.json
```js
    "repositories": [
        {
            "type": "vcs",
            "url": "https://github.com/colincode/server.git"
        }
    ],

```
```js
    "require": {
        "colincode/server": "dev-master"
    }

```
- Run composer update
```sh
composer update
```
- Run server-create in your project root folder
```sh
vendor/bin/server-create
```
##### Traditional
- Make sure you have Virtualbox, Vagrant & Ansible installed
- Install ubuntu trusty server
```sh
vagrant init ubuntu/trusty64
```
- Put the contents of this folder into your project root
- Bring up the server
```sh
vagrant up
```


# Composer installable LEMP server 

#### Vagrant config with Ansible provisioning for a LEMP server
#### Included Packages
- php5
- php5-mcrypt
- php-fpm
- mariadb
- nginx

#### Requirements
- [Virtualbox](https://www.virtualbox.org://www.virtualbox.org/)
- [Vagrant](https://www.vagrantup.com/)
- [Ansible](http://www.ansible.com/home)

#### How to use
##### VIA Composer
- Install ubuntu trusty server
```sh
vagrant init ubuntu/trusty64
```

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

- Bring up the server
```sh
vagrant up
```

#### .gitignore
Your .gitignore file will automatically be updated to ignore the Vagrant
& Ansible setup files/folders

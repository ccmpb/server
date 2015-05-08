# Vagrant & Ansible Webserver 

#### Vagrant config with Ansible provisioning for a LNMP server
#### Included Packages
- php5
- php-fpm
- mariadb
- nginx

#### How to use
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


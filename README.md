# install_php
Install php8.2 on centos7

1. sudo yum install epel-release
2. sudo yum install https://rpms.remirepo.net/enterprise/remi-release-7.rpm
3. php -v
  Check if any old php is already installed
  if any installed dissable remi for old version php 
5. sudo yum-config-manager --disable remi-php{PHP_VERSION}
if yum-config-manager not found then install yum utils: sudo yum install yum-utils

6.sudo yum-config-manager --disable remi-php{PHP_VERSION}
enable remi for new version
7.sudo yum-config-manager --enable remi-php82
8.sudo yum install php php-common php-cli
9.php -v

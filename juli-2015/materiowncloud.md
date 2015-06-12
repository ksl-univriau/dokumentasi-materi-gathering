# Install Owncloud Server di Debian/Ubuntu

- add repository owncloud 
`sudo sh -c "echo 'deb http://download.opensuse.org/repositories/isv:/ownCloud:/community/xUbuntu_14.04/ /' >> /etc/apt/sources.list.d/owncloud.list"`
`apt-get update`
- add key owncloud
wget http://download.opensuse.org/repositories/isv:ownCloud:community/xUbuntu_14.04/Release.key`
`sudo apt-key add - < Release.key  `
- install semua paket owncloud
`apt-get install owncloud`

# Database : `mariaDB`

Instalasi : `apt-get install mariadb-server`

# Setting database

`CREATE DATABASE owncloud`

kemudian berikan akses databse owncloud 

`GRANT ALL ON owncloud.* to 'owncloud'@'localhost' IDENTIFIED BY 'database_password';`

`exit`

akses ip address localhost : `localhost/owncloud`




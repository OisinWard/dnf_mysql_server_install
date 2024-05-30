# Non ansible build

## Instructions here

https://dev.mysql.com/doc/refman/8.0/en/linux-installation-yum-repo.html

## Commands

wget https://dev.mysql.com/get/mysql84-community-release-el9-1.noarch.rpm

sudo dnf localinstall mysql84-community-release-el9-1.noarch.rpm

dnf repolist all | grep mysql

systemctl start mysqld

sudo systemctl start mysqld

sudo systemctl status mysqld

sudo grep 'temporary password' /var/log/mysqld.log

mysql -uroot -p

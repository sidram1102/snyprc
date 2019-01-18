# Installation Prerequisites
#edit by sid
## MySQL

::: warning 
Before running the SNYPR product installer (SNYPR.bin), please make sure MySQL is pre-installed and configured on the Linux server (RHEL 7.x or CentOS 7.x). If some of these items are not installed or misconfigured, the installer will notify you during installation. Additionally, the Hadoop cluster is required after installation in order to configure the solution.
:::

### Install MySQL

MySQL 5.6+ can be used. This is used for configuration information. The SNYPR data is stored in Hadoop.

```sh
root> wget http://dev.mysql.com/get/mysql-community-release-el6-5.noarch.rpm

root> rpm –Uvh mysql-community-release-el6-5.noarch.rpm

root> yum install mysql-server
```
### Modify my.cnf file

```sh
root> vi /etc/my.cnf
```
```SQL
lower_case_table_names=1
```

### Set up MySQL to Start at Boot Time

```sh
root> chkconfig mysqld on
```

::: tip Note
You must update the my.cnf file if you are using MySQL version 5.7, and you receive the following error:
::: 

::: danger
To resolve this error, you must make the following change to the my.cnf file:
:::


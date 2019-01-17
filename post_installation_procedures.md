# Post Installation Procedures

## Spark Application Utility Script

When you have successfully installed SNYPR, complete the following steps to run the Spark jobs:

::: warning
Note: For complete details to run the scripts with different options, see the PFA readme file in /Securonix/tenants/snypr/Gateway/sparkJobs/readme_snypr_apps.txt.
:::

1. Navigate to the installation folder designated during Installation. Example: /Securonix/tenants/snypr/Gateway/sparkJobs/.
2. (Optional) Edit Spark jobs parameters in snypr_apps.properties file in /Securonix/tenants/snypr/Gateway/sparkJobs/conf/snypr_apps.properties.

```
snypr_apps.properties
``` 
- The scripts to run each spark job have been converted to accept the configurations as parameters
- Configurable parameters:

## Configure Redis

The redis.conf file contains a number of directives that have a very simple format: keyword argument1 argument2 ... argumentN.

Configure the following settings related to IP Address, Password, and Port for Redis from the redis.conf file. The path to the redis.conf file is determined during the installation process.

1. Bind the IP address to the server where Redis is installed. Example: bind 10.0.0.60
2. Accept connections on the specified port (default is 6379). Example: port 6379
3. Specify the password for the Redis. Example: requirepass open24X7

## Configure Syslog-ng
## Configure Hadoop
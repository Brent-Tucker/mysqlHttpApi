# mysqlHttpApi

## Requirements:

1. OpenResty has been installed under /usr/local/openresty, please refer to http://www.openresty.org/ for details.

2. MySQL has been installed.


## Usage:

1. Modify the MySQL settings in lua/appConfig.lua, the defaults are : host is localhost, port is 3306, database name is mysql, user name is root and password is root.

2. Start the app by running the shell file ./startup.sh, please modify the execution permission if it can't start. Please refer to OpenResty's documentation for how to start the service if you're using Windows to run OpenResty.

3. There is a single API, and access the url *http://localhost:6699/mysqlHttpApi/mysqlApi?sqlCmd=select * from user* to do the querying, remember to use HTTP POST method, and you can use any valid MySQL SQL command.

4. In your applications, you can use the above URL to do querying with MySQL, and should use HTTP POST to use the API.




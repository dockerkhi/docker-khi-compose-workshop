# Exercise 6

Create a WordPress website using Docker! For Wordpress we need 2 images `mysql:5.7` and `wordpress:latest`. 

MySQL needs the following ENVs configured:
```
MYSQL_ROOT_PASSWORD: somewordpress
MYSQL_DATABASE: wordpress
MYSQL_USER: wordpress
MYSQL_PASSWORD: wordpress
```

WordPress needs the following environment configured:
```
WORDPRESS_DB_HOST: db:3306
WORDPRESS_DB_USER: wordpress
WORDPRESS_DB_PASSWORD: wordpress
WORDPRESS_DEBUG: 1
```

WordPress is served via Apache (httpd) so container port is `80`.

Bonus: You can configure ENV Variables from your shell inside your Docker file. So if you have a $DB_USER configured as an ENV variable in your shell, you can use the ${DB_USER} syntax to provide the value. You can also use a .env file to provide the default value as well.